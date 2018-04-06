Après avoir rédigé [mon article décrivant le fonctionnement du Ledger Wallet Nano S](https://steemit.com/crypto/@iero/ledger-wallet-comment-ca-marche), je suis tombé sur deux nouveaux produit fabriqués par **Kapersky Labs**, l'éditeur d'antivirus bien connu : le [Ballet et le Securator](https://wallet.kaspersky.com/).

![kapersky.png](https://steemitimages.com/DQmSvCAF78GPWU8NqQMaAPetVs2ayPR1XK7pG9jyuzPQMve/kapersky.png)

Avant d'aller plus loin, si vous voulez comprendre l'intérêt et le fonctionnement d'un **hardware wallet**, (portefeuille physique) et pourquoi il faut absolument en avoir un pour sécuriser ses cryptos, [lisez mon article sur le ledger](https://steemit.com/crypto/@iero/ledger-wallet-comment-ca-marche).

## Les produits

Comme le montre l'image plus haut, les deux devices ressemblent à des vieilles clés USB. Le **Ballet** est le plus simple et coute $25. Le **Securator** coute quatre fois plus cher ($99), est légèrement plus gros et contient en plus un écran et une prise lightning (iPhone).

Le design présenté n'est peut-etre pas le final mais de ce qu'on peut y voir :

* Tous deux sont équipés d'une prise USB fixe (comme sur les vieilles clés USB). Il faudra un adaptateur pour pouvoir les utiliser sur des machines récentes équipées d'USB-C ;
* On ne peut pas attacher un cordon (très utile pour ne pas perdre la clé)
* Le micro-controleur a l'air classique, et équivalent au *ST31/STM32*. S'ils avaient mieux (comme la certification *CC EAL5+* du Ledger) ils l'auraient spécifié.
* Ils ont prévu (mais pas développé encore vu la mauvaise qualité des captures d'écran) une application iOS pour interagir avec un iPhone (et sûrement Android aussi) par communication sans-fil en NFC ou directe par prise lightning pour le **Securator**. Vu le [faible niveau d'ouverture de Core NFC sur iPhone](https://www.igen.fr/iphone/2017/06/core-nfc-apple-ouvre-un-peu-la-nfc-de-liphone-100106), j'ai un gros doute sur la capacité de Kapersky de pouvoir proposer du sans-fil pour les téléphone Apple. Ce qui voudrait dire que seul la version 'luxe' serait compatible avec un iPhone.
* Il n'est pas mentionné d'application Mac, Linux ou Windows, ni de compatibilité avec [MyCrypto](https://www.mycrypto.com). Est-ce qu'on devra se connecter sur une instance propriétaire Kapersky pour effectuer des transactions ? J'en ai peur.

Les Kapersky supportent **peu de monnaies** par rapport à la vingtaine du ledger, mais **les principales y sont** : Bitcoin, Bitcoin Cash, Ethereum, Ethereum Classic, Litecoin, Dash, Zcash, Ripple. Ils envisagent de rajouter le Bitcoin Gold, Monero et le Dogecoin.

![hain.png](https://steemitimages.com/DQmY3zbC1uT8jPwtsBt4GAUDytauhbRtp5GV5NvTSMsZjZN/hain.png)

Enfin, il y a une proposition de souscrire à "blockvault", un service premium (facturée $30 par an) permettant de faire une copie "hors ligne" du device. Il y a peu de détails sur cette option, mais si c'est pour pouvoir copier sa clé privée (la fameuse passphrase de 24 mots) chez Kapersky, c'est une **très mauvaise idée d'un point de vue sécurité**. La meilleure (seule) manière de sécuriser ce sésame étant de le mettre par écrit dans un coffre ou d'utiliser des moyens exotiques comme de la [stéganographie](https://fr.wikipedia.org/wiki/St%C3%A9ganographie). Surtout pas de le confier à un tiers numérique !

## Mon avis

Comme [Archos](https://www.numerama.com/tech/331640-cryptomonnaies-archos-a-t-il-les-moyens-techniques-et-materiels-de-se-rever-en-ledger.html), Kapersky utilise sa marque pour vendre un nouveau produit et surfer sur le buzz des crypto-monnaies : Ils annoncent qu'ils proposent le **premier** device créé par des *professionels en cybersecurité* alors que les équipes de [Ledger](https://www.ledgerwallet.com/) ou [Trezor](https://trezor.io/) étant exclusivement sur ce sujet depuis plusieurs années, je les considère comme des professionels aussi.

Kapersky labs a fait l'objet de nombreuses polémiques ces derniers mois, avec des [accusations d'espionnage](http://www.lemonde.fr/pixels/article/2017/10/11/la-russie-accusee-d-avoir-utilise-l-antivirus-kaspersky-pour-espionner-la-nsa-americaine_5199375_4408996.html) pour le compte du gouvernement Russe. [Leurs produits ont été interdits par décret](https://www.reuters.com/article/us-usa-cyber-kaspersky/trump-signs-into-law-u-s-government-ban-on-kaspersky-lab-software-idUSKBN1E62V4) au sein du gouvernement US, et, même s'ils ont de très bon ingénieurs, cette société a perdu la confiance de nombreux utilisateurs.  
Leur proposition de *'BlockVault'* me semble dangereuse et ne semble pas aller dans le sens de la sécurité.

Après de longues années de calme, des failles de sécurité visant Ledger [ont fait la une des journeaux](https://cointelegraph.com/news/teenager-who-hacked-ledger-hardware-wallet-says-devices-still-vulnerable-devs-deny) ces dernières semaines, mais [l'équipe a une excellente communication, très transparente](https://www.ledger.fr/2018/03/20/firmware-1-4-deep-dive-security-fixes/) et ont publié un fix très rapidement. Ils ont aussi une [politique de bug bounty très agressive](https://www.ledger.fr/bounty-program/).

Tout ceci représente donc un important **gage de confiance**, et il est clair qu'aujourd'hui le [Ledger](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT) est encore le meilleur choix pour protéger vos Cryptos, et rien ne justifie à ce stade de se positionner sur un Kapersky.