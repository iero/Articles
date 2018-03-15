![iexec.jpg](https://steemitimages.com/DQmWpAdbQtXzQGCjq2nun2biXnDRqzvqn8ZftK5PHk62mx5/iexec.jpg)

[iExec](https://iex.ec/fr/) fait régulièrement les titres de différents sites dédiés aux cryptomonnaies ces derniers jours. C'est un projet franco-chinois porté par une startup Lyonnaise et accéléré par l’Université de Tsinghua (Pékin) ayant pour objectif de **boulverser le calcul décentralisé** en proposant un réseau capable d'exécuter le code contenu dans les [smart-contrats d'Ethereum](https://www.ethereum-france.com/quest-ce-quune-dapp-quelques-exemples-simples/).

## Comment ca marche

[iExec](https://iex.ec/fr/) veut proposer une place de marché mettant en relation les fournisseurs de ressources de calcul (sociétés ou particuliers) et ceux qui en ont besoin. Les prix des calculs ne seront pas dictés par quelques sociétés, mais sera variable, et négocié en fonction de l'offre et de la demande.

![1_JX3qpUo61hqHoAqHu8OoyA.png](https://steemitimages.com/DQmRownbh8cipS8HUu76XqSC2cpciJp71RXVP1nMfvRAjbj/1_JX3qpUo61hqHoAqHu8OoyA.png)

Sur la blockchain Ethereum, les applications décentralisées, appelées [dApps](https://www.ethereum-france.com/ecrire-une-dapp-pour-ethereum-1-smart-contract/), permettent d'éxécuter du calcul à partir de smartcontrats.

Les dApps sont composées de deux parties : l'*interface utilisateur* et le *backend*. Dans le cas d'Ethereum, le code backend, contenu dans les *smart-contrats*, s'exécute sur le réseau peer-to-peer décentralisé global Ethereum et les interfaces utilisateur, pouvant être écrits dans n'importe quelle language, y font appel.

> dApp = interface utilisateur + smart-contrat

Ici, l'idée est donc de sous-traiter, contre rémunération, ces calculs sur des serveurs dédiés.

![1_2ptDUR3JcPFOrZgSa8onag.png](https://steemitimages.com/DQmRb3cgT121PzaEFQXU4NTC7RKQjHWGj2Qu3az4Su79Hnk/1_2ptDUR3JcPFOrZgSa8onag.png)

Comme [j'ai déjà expliqué sur mon analyse de Cardstack](https://steemit.com/ico/@iero/ico-cardstack-card-analyse) une poignée d'acteurs se partagent aujourd'hui Internet. Dans le cas du cloud computing, les acteurs principaux, comme [AWS](https://aws.amazon.com/), [GCP](https://cloud.google.com/), [Alibaba](https://www.alibabacloud.com/) et [Azure](https://azure.microsoft.com/fr-fr/) proposent des dizaines de briques, allant du stockage de données (store) à l'execution de code (compute), avec une importante panoplie de services associés (machine learning, analytics, etc). 

Pour chaque nouveau projet qui se crée, il est bien plus facile (et moins cher) d'utiliser ces briques existantes que de monter son propre datacenter, le configurer, l'optimiser et de le maintenir. Mais cette facilité entretient la dépendance que nous avons vis-à -vis de ces gros acteurs. Ils ont aujourd'hui une telle avance, aussi bien en propriété intellectuelle, qu'en ressources (humaines ou machine), qu'aucun acteur Européen n'est capable de les rattraper.

Dans une dApp, on peut insérer n'importe quel calcul : par exemple, un projet scientifique comme [Seti@Home](https://setiathome.berkeley.edu/), du calcul de rendu 3D ou du calcul sur GPU.

![1_ZG2Hb1DmduNVh4Ch_xKKDg.png](https://steemitimages.com/DQmXkB6G2vxCvNAFx7iopDxEzQXtan3mR3qeXteJ52adQWD/1_ZG2Hb1DmduNVh4Ch_xKKDg.png)

Coté architecture, iExec contient :

* une **marketplace** pour mettre en relation les fournisseurs de ressources de calcul et les utilisateurs de dApp
* un **store** pour trouver la dApp de ses rêves
* un **data marketplace** pour vendre/acheter de la donnée

Coté technique, le calcul sera supporté et distribué par [XtremWeb-HEP](https://xtremweb-hep.lal.in2p3.fr/), un logiciel de gestion de grille open-source créé il y a une dizaine d'années [par le CNRS et l'Inria](https://medium.com/iex-ec/understanding-the-technology-behind-the-iex-ec-distributed-cloud-d91965fff00a). 

## Token (RLC) :

Le **RLC** (*Runs on Lots of Computers*) est un *utility token ERC20* permettant d'acheter ou de vendre de la ressource de calcul sur la plateforme.

Il y a 87 millions de tokens en circulation, dont 60 M ont été vendu pendant l'ICO (pour 12M d'euros). Depuis son entrée sur les différents exchanges, le RLC a vu sa valeur baisser, puis augmenter très fortement pendant le mois de mars 2018 pour se restabiliser autour de 0.00013 BTC.

![coinmarketcap.png](https://steemitimages.com/DQmWbgV775ZzMjfDshghrqBNToRMRFnWugFivFyW7GKqhi6/coinmarketcap.png)

## Pourquoi ca peut marcher ?

L'équipe est constituée de très bons profils connaissant les réseaux distribués et ayant déjà travaillé depuis une dizaine d'années sur ces sujets à l'Inria, au CNRS ou à l’Académie des Sciences de Chine.

iExec est **indispensable pour garantir l'avenir d'Ethereum**. Actuellement le code dans les smart-contrat est exécuté par les mineurs à chaque validation d'un nouveau bloc. Mais la puissance demandé étant croissante, il faudra rapidement sous-traiter cette exécution à des serveurs spécialisés pour ne pas ralentir la blockchain.

Plusieurs acteurs sont sur ce créneau, comme [Enigma](https://enigma.co/), [Siacoin](https://sia.tech/) (stockage), [Truebit](https://truebit.io/), [SONM](https://sonm.com/) ou [Golem](https://golem.network/) (High Performance Computing, calcul lourd). Mais iExec est **le seul à proposer une solution déjà fonctionelle, permettant l'execution des dApps**. 

La [roadmap](https://iex.ec/fr/roadmap/) est ambitieuse et la prochaine version majeure de iExec (v2) est prévue pour la fin du mois de mai 2018. Le prix du token devrait bien monter à ce moment là..

## Pour aller plus loin

* Le [whitepaper](https://iex.ec/app/uploads/2017/04/iExec-WPv2.0-English.pdf)
* L'équipe est disponible sur [Twitter](https://twitter.com/iEx_ec), [slack](http://slack.iex.ec/) ou [Telegram](https://t.me/iexec_announcements)
* Une [bonne explication](https://coincentral.com/iexec-rlc-beginners-guide-decentralized-cloud-computing/) en anglais
* Un excellent [article sur hackernoon](https://hackernoon.com/blockchains-need-iexec-the-market-just-hasnt-realized-it-yet-5597c743cd0a)

### @iero

Pas de compte steemit pour *liker* ? Vous pouvez m'envoyer quelque poussières d'ethereum à cette adresse  *0xEeCAf0dCB3a870d84Ad851D66514169B11968020*