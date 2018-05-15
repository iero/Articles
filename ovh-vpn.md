# Tunnel VPN sur OVH

Pourquoi OVH ? Car les VPS sont vraiment pas chers *(3,59 €/mois TTC lors de l'écriture de cet article)*, avec une bonne bande passante (100Mbps) et surtout un **traffic illimité**.

# Prerequis

Sur [la page d'OVH](https://www.ovh.com/fr/vps/) sélectionnez un `VPS SSD`  

J'ai installé `Ubuntu 16.04` en anglais car la dernière version (bionic 18.04) n'avait pas tous les paquets.

# Installation du système 

Une fois le mail reçu avec le nom de votre serveur (vpsXXXXXXX) et vos identifiant, connectez vous :

    $ ssh root@vpsXXXXXX

Une fois connecté, on change son mot de passe root, puis on met à jour la distribution. Sélectionnez **Y** pour confirmer la mise à jour, puis **N** pour garder la version OVH de `/etc/cloud/cloud.cfg`

	passwd
    apt-get update
    apt-get upgrade
    
Supprimer l'utilisateur par défaut `ubuntu`, puis ajouter un groupe, un utilisateur et lui mettre un mot de passe :

	userdel ubuntu
	rm -rf /home/ubuntu
	groupadd iero
    useradd -g iero -m -s /bin/bash iero
	usermod -a -G sudo iero
    passwd iero
    
    sudo ssh-keygen -A
    
Dans `/etc/ssh/sshd_config`, interdire root de se connecter :

    PermitRootLogin no

Générer (à faire une fois) et copier sa clé privée sur le vps :

    ssh keygen
    ssh-copy-id -i ~/.ssh/id_rsa.pub iero@vpsXXXXXXX

## Optionel : Si vous avez un nom de domaine

Modifier `/etc/cloud/cloud.cfg` :

    disable_root: 1
    preserve_hostname: true
    manage_etc_hosts: false

Mettre le bon hostname dans `/etc/hostname` et mettre à jour `/etc/hosts`
	
# Configuration :

On installe les paquets nécessaires. Sélectionnez **Yes** pour garder les configuration iptables existantes :

    sudo apt-get install strongswan strongswan-plugin-eap-mschapv2 moreutils iptables-persistent


Créer les certificats VPN :    

    mkdir vpn-certs
    cd vpn-certs    
    ipsec pki --gen --type rsa --size 4096 --outform pem > server-root-key.pem
    chmod 600 server-root-key.pem

    ipsec pki --self --ca --lifetime 3650 \
> --in server-root-key.pem \
> --type rsa --dn "C=EU, O=Rebel, CN=Rebel Root CA" \
> --outform pem > server-root-ca.pem
> 
> 

On crée les certificats serveur :

    ipsec pki --gen --type rsa --size 4096 --outform pem > vpn-server-key.pem

    sudo ipsec pki --pub --in vpn-server-key.pem \
    --type rsa | ipsec pki --issue --lifetime 1825 \
    --cacert server-root-ca.pem \
    --cakey server-root-key.pem \
    --dn "C=EU, O=Rebel, CN=rebel.iero.org" \
	--san rebel.iero.org \
	--flag serverAuth --flag ikeIntermediate \
	--outform pem > vpn-server-cert.pem
    
    sudo cp ./vpn-server-cert.pem /etc/ipsec.d/certs/vpn-server-cert.pem
    sudo cp ./vpn-server-key.pem /etc/ipsec.d/private/vpn-server-key.pem


    sudo chown root /etc/ipsec.d/private/vpn-server-key.pem
    sudo chgrp root /etc/ipsec.d/private/vpn-server-key.pem
    sudo chmod 600 /etc/ipsec.d/private/vpn-server-key.pem

    sudo cp /etc/ipsec.conf /etc/ipsec.conf.original
    echo '' | sudo tee /etc/ipsec.conf


/etc/ipsec.conf

config setup
      charondebug="ike 1, knl 1, cfg 0"
      uniqueids=no

      conn ikev2-vpn
  auto=add
  compress=no
  type=tunnel
  keyexchange=ikev2
  fragmentation=yes
  forceencaps=yes

  ike=aes256-sha1-modp1024,3des-sha1-modp1024!
  esp=aes256-sha1,3des-sha1!

  dpdaction=clear
  dpddelay=300s
  rekey=no
 
  left=%any
  leftid=@rebel.iero.org
  leftcert=/etc/ipsec.d/certs/vpn-server-cert.pem
  leftsendcert=always
  leftsubnet=0.0.0.0/0

  right=%any
  rightid=%any
  rightauth=eap-mschapv2
  rightsourceip=10.10.10.0/24
  rightdns=8.8.8.8,8.8.4.4
  rightsendcert=never

  eap_identity=%identity


    rebel.iero.org : RSA "/etc/ipsec.d/private/vpn-server-key.pem"
    your_username %any% : EAP "your_password"
    
    sudo ufw disable
    
    sudo iptables -P INPUT ACCEPT
sudo iptables -P FORWARD ACCEPT
sudo iptables -F
sudo iptables -Z
sudo iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
sudo iptables -A INPUT -p udp --dport 60000:61000 -j ACCEPT
sudo iptables -A INPUT -i lo -j ACCEPT
sudo iptables -A INPUT -p udp --dport  500 -j ACCEPT
sudo iptables -A INPUT -p udp --dport 4500 -j ACCEPT
sudo iptables -A FORWARD --match policy --pol ipsec --dir in  --proto esp -s 10.10.10.10/24 -j ACCEPT
sudo iptables -A FORWARD --match policy --pol ipsec --dir out --proto esp -d 10.10.10.10/24 -j ACCEPT
sudo iptables -t nat -A POSTROUTING -s 10.10.10.10/24 -o ens3 -m policy --pol ipsec --dir out -j ACCEPT
sudo iptables -t nat -A POSTROUTING -s 10.10.10.10/24 -o ens3 -j MASQUERADE
sudo iptables -t mangle -A FORWARD --match policy --pol ipsec --dir in -s 10.10.10.10/24 -o ens3 -p tcp -m tcp --tcp-flags SYN,RST SYN -m tcpmss --mss 1361:1536 -j TCPMSS --set-mss 1360
sudo iptables -A INPUT -j DROP
sudo iptables -A FORWARD -j DROP
sudo netfilter-persistent save
sudo netfilter-persistent reload


/etc/sysctl.conf

    net.ipv4.ip_forward=1
    net.ipv4.conf.all.accept_redirects = 0
    net.ipv4.conf.all.send_redirects = 0
    net.ipv4.ip_no_pmtu_disc = 1
    
    
scp iero@rebel.iero.org:/home/iero/vpn-certs/server-root-ca.pem .

# Divers

Install Mosh

    sudo apt-get install mosh


Anaconda

wget https://repo.anaconda.com/archive/Anaconda3-5.1.0-Linux-x86_64.sh
    
    
    