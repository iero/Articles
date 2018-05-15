ICO - Sergio

# Quarkchain

Projet Infrastructure - protocole de premier niveau.

## Base

Les projets Blockchain se basent sur trois piliers :

* **Sécurité** : Le réseau s'assure que chaque transaction est valide et soit être resistant aux attaques ;
* **Décentralisé** : Personne ne peut en prendre controle du système, et donc être capable de le corrompre ;
* **Passage à l'échelle** (scalabilité) : Le prix et le temps de transaction n'augmentera pas avec le nombre d'utilisateurs.

En une seconde, les systèmes suivants permettent :

* Bitcoin : 7 transactions
* Ethereum : 15 transactions
* Visa : 60 000 transactions
* Alipay : 200 000 transactions

Les blockchains les plus connues, le Bitcoin et l'Ethereum ont été conçues pour être sûres et décentralisées. Même si ce deuxième point est discutable (plus de la moitié du minage mondial du bitcoin est réalisé par une poignée de sociétés de minage), leur point faible est clairement le passage à l'échelle.

Pour contourner cette limitation, Bitcoin travaille sur le Lighning Network, qui permet d'enregistrer des packets de transactions sur la blockchain plutôt que chaque transaction, et Ethereum travaille plutôt sur le concept de Sharding (?? protocole de consensus permettant de casser la blockchain principale en multiples).

D'autres blockchains ont fait le choix de dégrader la sécurité (exemple) ou la décentralisation (Ripple) pour pouvoir gagner sur les deux autres axes.

## La réponse de Quarkchain

Quarkchain veut être décentralisé, sûr et rapide. Pour cela, cette blockchain se base sur deux couches : Une blockchain mère et des blockchains filles.

Les blockchains filles permettent de connaitre le **solde d'un compte** et **met à jour ce solde** pour chaque transaction valide. Elles sont dites **shardées** car chacune ne gère qu'un petit nombre des transactions totales et **elastiques** car leur nombre peut augmenter ou diminuer en fonction de l'activité. 

Une fois la transaction validée, les **entêtes des transactions** sont êcrites (par paquets) sur la blockchain mère.

L'existence de cette double couches avec des blockchains shardées élastiques permet de garantir le passage à l'échelle et de réaliser 1 million de transactions par seconde.

Comme Monero, Quarkchain utilise un système de *Proof Of Work* résistant aux systèmes ASICs.

La difficulté de minage variable est variable, aussi bien pour la blockchain mère que pour les blockchains filles. Toutes ces blockchains proposent leur difficulité de minage et les gains associés sur sur une sorte de place de marché ou chaque mineur, qu'il soit petit ou puissant, pourra choisir quel block miner. Le système permet de distribuer la difficulté globale avec au moins 50% sur la blockchain mère. 
Le minage par équipe n'est donc pas encouragé par une probabilité de gain plus forte. Tout celà permet de garantir une meilleure décentralisation que les systèmes existants.

Pour trouver rapidement la trace des comptes répartis sur toutes les blockchains filles, chaque utilsateur utilise un compte principal (Primary Account) qui sert de tampon entre ses différents comptes et un portefeuille intelligent (Smart Wallet) qui permet de réaliser les transactions entre les différentes chaines.

> A malicious user looking to attack QuarkChain requires at least 25% of the network’s total hash power, which is less than the 51% required for Bitcoin.

Clustering : Pour éviter que seuls les acteurs ayant une grande bande passante et beaucoup de stockage puissent valider un grand nombre de transaction par seconde (10Gb de bande passante et 10Tb de stockage pour 500 000 transactions par seconde), Quarkchain permet aux petits mineurs de se regrouper en mini-nodes permettant de former des full-nodes (entité de minage ayant une copie complète de la blockchain).

## Smartcontrats

Il y aura un système de smart-contrats et les développeurs Ethereum pourront porter facilement les dApps sur ce système.

Tres gros ROI  
private sale 16M de dollar, 4M pour la sail. 
Tres petit Marketcap.
Tres peu de token dans les exchanges car ils sortiront petit à pett.

Blockchain de test deja en fonction

Superbe team : instagram, google, facebook

# Edenchain

ROI enorme

Ya un mvp

# Loki 

Fork de Monero
snaps : applications qui tournent au dessus
Tom Windget de Monero

Tres petit hardcap : 9M$
Pas mal de token minés la première année.

Potentiel x5 à x10 à la sortie

# Bezant

Bezant est arrivé au hardcap en quelques minutes pendant la pre-sale
A prendre pendant la sortie sur exchanges

# Certik

Audit sur les smartcontrats : Tres important.
Très bonne team venant de l'université, mais peu qui viennnent du business ou developement.
Certik a un prix 4 à 5x plus haut que coinstamp
Algos qui vont verifier le code de manière automatique
deja une demo qui marche

Bientot une whitelist ?

# OriginProtocol (Genesis).

Yu Pan de paypal dans la team.
Crowdsale en Q2 2018 ? Whitelist bientot ?

Superbe projet

# Atonomi

Tres bon projet à garder à l'oeil. 
Whitelist

# Steem

## Blockchain Steem

Steem est une blockchain qui propose aux projets un système de *récompenses*.

Steem peut gérer jusqu'à 10 000 transactions/sec. Il n'y a pas de frais de transaction, mais un *fair use* pour éviter le spam.

L'adresse publique est le pseudo (Par exemple @iero pour moi). On ne peut donc pas le changer.

Pour chaque compte, il y a trois clés privés associés :

* Clé **posting** : utilisée pour poster, commenter, liker
* Clé **active** : pour transferer les fonds
* Clé **owner** : permet de regénérer les deux autres clés

Pour protéger ces clés sur la plateforme, un master password : permet de crypter ces clés (16 caracteres ?)

La validation des blocks se fait via un système de *Proof Of Brain* qui est un mélange de **Proof of Work** (Mining, appelé Witness, 10%) et **Proof Of Stakes** (15% redistribué aux porteurs de SP et le reste aux créateurs de contenus/commentaires)

Le STEEM est une monnaie inflationiste avec une inflation d'un peu moins de 10% au lancement, en baisse régulière jusqu'à un peu moins d'1% pendant 20 ans.

Les récompenses sont des **SMT** (Smart Media Token). 

## Smart Media Tokens 

Le SMT permet donc de créer des tokens sur cette blockchain comme ERC20 le fait sur Ethereum.

Les tokens SMT actuels sont :

* STEEM : Token de récompense principal
* STEEM POWER (SP) : Ce sont des tokens STEEM bloqués pendant 3 mois.
* STEEM Backed Dollars (SBD) : Ce token ne tombera pas en dessous de 1 USD. 

## Steemit

**Steemit est actuelement le projet principal** utilisant cette blockchain. Son objectif est de proposer une plateforme de blog permettant de rémunérer les auteurs de contenu, qu'ils soient les auteurs principaux, ou des commentateurs utiles.

On peut donc la comparer à un Medium ou un Reddit décentralisé.


## Problèmes fonctionnels : 

l'inscription est gratuite pour l'utilisateur, car pris en charge par la communauté (A VERIFIER). Mais pour éviter les abus, le processus est long et fastidieux (de quelques heures à quelques semaines). Ca n'aide pas les nouveaux utilisateurs qui voudraient juste *liker* ou *suivre* à franchir le pas et à rejoindre la plateforme.

Les premiers utilisateurs actifs de cette plateforme ont historiquement beaucoup de SP (les baleines) qui leur permet de rémunérer d'autre utilisateurs en likant leur contenu (upvote). Certains utilisent cette puissance pour vendre leurs votes.

Il y a un système de bots mettant des votes ou des commentaires automatiques qui déstabilise le système originel.

Ces systèmes sont cependant utilisés par des regroupements de baleines bienveillantes pour aider les petits porteurs (appelé plancton) à monter en grade.

Les interfaces (frontend) sont pauvres, mélangeant les posts de qualité aux posts manipulés par les bots/baleines à ceux sans intérêts. La seule solution que proposent Steemit/Busy pour éviter ce flux est de s'abonner à des sources. 

Enfin, la plateforme est encore jeune et utilisée massivement par la faible population des crypto-maniaques. Sa complexité fait qu'elle manque de visibilité en dehors de cet écosystème.

## Conclusion

IRC est un protocole de communication, utilisé dans les années 90 et 2000 pour discuter sur des thèmes dans des salles de discussions. Techniquement, IRC était parfaitement réalisé et permettait de connecter un grand nombre de personnes entre elles. Mais, comme Steem, sa complexité ne l'a laissé à la porté que de l'écosystème de geeks (dont je faisais partie). Il a cependant fallu attendre le milieu des années 2010 pour que Slack (et d'autres, comme Discord), s'approprient ce système et le fasse évoluer en un outil propriétaire convivial et utilisable par le plus grand nombre. Le nombre d'utilisateurs a explosé et un business model autour de segments non-geeks (entreprises, gamers) s'est créé.

Nous avons ici la même situation. Le système est là, plutôt bien conçu et fonctionnant plutôt bien. Mais comme IRC dans son temps, il n'est utilisé que par des early-adopters et n'a quasiment aucune chance de décoller en l'état.

Cependant, le système de SMT ne demande qu'à évoluer pour qu'un acteur, ou un groupe d'acteurs, puisse mettre en place une plateforme simple, décentralisée et  

## Autres projets :

Publiq Media (actuellement en testnet) https://publiq.network/﻿

## Sources :

Vidéo explicative de CoinTips
https://www.youtube.com/watch?v=kndEKX1s8_w

# Cardano

Cryptomonnaie de 3e génération lancée en sept 2017 apres plus de 2 ans de dev.

Premiere génération : bitcoin. Une seule application : monnaie digitale
Deuxième génération : ethereum. Plusieurs applications (dApps)
Troisième génération : Ada, iota, EOS

Problème de scalabilité, bande passante et stockage.

Elle a des peer-reviewer pour discuter scientifiquement des papers pour résoudre des problèmes. Grosse équipe diversifiée et qualifiée.

Consensus Proof Of Work permet de prouver (sécurisé) mais est peu scalable. Gros couts énergétiques (inutile) et centralisation (entreprises).

Proof Of Stake : Au lieu d'allouer une puissance de calcul, on alloue des ADA.

Une epoch (20h) avec 600 slots de 20sec. Cardano va choisir aleatoirement 600 personnes qui vont créer chacun leur block.

Il est possible d'avoir des epochs en parallèles pour pouvoir augmenter le nombre de block.

On peut aussi faire du dPOs (delegated Proof Of Stake). On peut déléguer notre pouvoir de minage à une pool.

Plus on augmente le nombre de transactions, plus on augmente la bande passante pour que tout le monde puisse avoir les infos pour pouvoir valider les blocks.
Rina : sous-reseaux dans des groupes qui communiquent entre eux.

Taille ? En cours de resolution

## NiPoPoW

Sidechain : Paiement d'un coté, et smartcontract d'un autre (deux chaines). On pourra connecter la partie paiement avec bitcoin/ethereum.

Durabilité/modèle économique pour s'auto-financer.
Cardano récupère par smartcontrat des poussières de transactions. L'équipe de Cardano va mettre un projet au vote (des porteurs de Cardano), et les fonds seront débloqués.

Dans chaque transaction, on pourra (ou non) mettre des infos de la source, la destination et la raison (pour être compatible avec le système bancaire).

## Cardano

IOHK : Entreprise en charge du dévelopement de la blockchain. Contrat jusqu'en 2020 
Fondation : Création de standards au niveau de la blockchain (pour interoperabilitéà
Emurgo : partenariats, incubations, business.

Roadmap ???
Gros potentiel s'ils arrivent à délivrer.

ils vont faire des dApps compatibles avec Ethereum

Deux ICO en cours sur Cardano (Traxia - gestion des factures impayés, Sp8de - casino en ligne), et des business qui arrivent. Plus des cartes de paiements.

Ya une guerre entre Ethereum, Cardano et EOS.

Vidéo explicative de CoinTips
Source : https://www.youtube.com/watch?v=wqUsHtLcciA

# EOS

Blockchain de 3e génération
Longue ICO avec des mises aux enchères chaque mois

Charte d'utilisation du réseau pour les applications (dApps). Système de vote
Pas de frais de transaction (comme le iota).

Pour faire des transactions, il faut stocker des IOS.
Inflation au max de 5% par an, sans maximum.

On pourra modifier un smartcontrat par un systeme de vote. Pas besoin de hardfork si il y a un pb

Adresse publique personalisée 
Compatible ethereum pour les smartcontrats.

Objectif de 1 million de transaction par seconde 

## Proof of Stake 

21 producteurs pour commencer.
Contraintes pour les producteurs afin que ca soit rapide. Ils vont se faire élire 

Blockchains en parallele comme sur Cardano.

EOS deja à 10 USD. 6e sans aucun produit encore.
MainNet prévu en juin. Assez confiant car l'équipe est bonne.

Gros potentiel. Ils ont levé 2.5 Milliards. Pour faire des partenariats ?

Partenariat avec Finlab, Galaxy et BitFinex

