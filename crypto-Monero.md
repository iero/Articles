![monero.png](https://steemitimages.com/DQmdLeSidWCWpjgYJGTXoPEqE2ADexbahNmUJFHjd6cxUQb/monero.png)

Le Monero, alias XMR est une crypto-monnaie surtout connue pour être :

* la monnaie anonyme des trafiquants et marchands d'armes ;
* le moyen de [miner sur les ordinateurs à l'insu des utilisateurs](https://www.ccn.com/pirate-bay-resumes-mining-monero-using-visitor-cpu-power/)

Mais cette monnaie n'est pas seulement utile pour les personnes ayant des choses à cacher, elle l'est aussi pour celles ayant envie de **protéger leur vie privée**. 

Bitcoin, ethereum, et les autres monnaies classiques ne garantissent pas l'anonymat d'une transaction. Il suffit que je vous donne mon *adresse publique* pour que vous connaissiez toutes le transactions (montant, source et destination) qui y sont passées. Vous pourrez donc savoir **ce que j'ai acheté**, pour **combien**, et **avec qui** j'ai échangé de l'argent.  
C'est un peu comme si vous me donniez **accès à vos relevés bancaires**.

![eth.png](https://steemitimages.com/DQmbdyrhhs169NmaqmkE8WqV2uD5CxtRUogeWZxLsZBmECf/eth.png)

Monero utilise un mécanisme d'obfuscation et des adresses furtives permettant de pouvoir anonymiser les transactions. La technologie du Monero est très avancée et reconnue par de nombreux spécialistes. Le code source étant ouvert, de [nombreux articles](https://en.wikipedia.org/wiki/Monero_(cryptocurrency)) entrent dans les détails de son fonctionnement. Pour résumer, Monero est :

* **Sûr** grâce à son réseau décentralisé utilisant le système de *proof of work (PoW)*. Son code est opensource, et résistant au minage ASIC (architecture utilisé pour minage du bitcoin). Ceci permet d'avoir un très grand nombre de mineurs, et non pas une concentration de quelques fermes de minages spécialisées ;
* **Privé** grâce à son système de *ring signatures* permettant de masquer les montants, l'origine et la destination de toutes les transactions ;
* **Intraçable** car les transactions sur la blockchain Monero ne permettent pas d'identifier un utilisateur ;
* **Fongible** car [un Monero n'est jamais sale](http://www.bitcoincours.com/2017/01/monero-xmr-reussit-devenir-fongible.html). Ne pouvant pas retracer le parcours d'un jeton, il ne pourra jamais être considéré comme issu d'une transaction douteuse et donc bloqué par un établissement.

## Investissement long terme

Dans le cadre d'un investissement long terme, je ne souhaite pas mettre tous mes espoirs sur les crypto-monnaies classiques, et je préfère diversifier en utilisant aussi dest alts comme Neo, Cardano et Monero.

**Pourquoi le Monero ?** Car c'est tout d'abord une monnaie solide, largement utilisée, avec un market cap de 3 milliards USD (11ème monnaie actuellement).
Elle a une vraie utilité, car c'est la seule permettant un réel anonymat. Elle peut donc servir par exemple aux journalistes ou aux utilisateurs vivant dans des pays ayant des politiques anti-crypto. Si toutes les monnaies deviennent traquées ou controlées, alors le Monero deviendra le **refuge ultime**.

De plus, les caractéristiques du Monero sont testées par [plusieurs sites](https://www.salon.com/about/faq-what-happens-when-i-choose-to-suppress-ads-on-salon/) pour pour remplacer les publicités par du minage dans le navigateur. Cette méthode semble en pleine expansion, et il commence même à y avoir [des applications sur l'App store](https://www.theverge.com/2018/3/12/17110810/apple-app-store-mac-cryptocurrency-monero-calendar-2-qbix) qui utilisent ce procédé pour se rémunérer.

## Comment l'utiliser ?

Pour faire simple, il y a deux méthodes pour créer votre portefeuille Monero :

[Monero wallet](https://getmonero.org/downloads), disponible en version *ligne de commande* ou *client graphique* est assez simple d'usage. Mais pour l'utiliser, il faudra synchroniser la totalité de la blockchain, c'est à dire actuellement **44Go** de blocks (environ 2 jours de téléchargement sur une ADSL, puis quelques minutes de synchronisation chaque jour) :

    $ ls -hl ~/.bitmonero/lmdb/data.mdb 
    44G 18 mar .bitmonero/lmdb/data.mdb 

C'est fastidieux, mais une fois installé, l'interface est classique et fonctionnelle. 

![gui.png](https://steemitimages.com/DQmRtShzxFS8gg3jYr4628wHsnBpPu5cVCoHX9ZYhm68Dev/gui.png)

[Mymonero](https://mymonero.com) est un web-wallet maintenu par [Riccardo Spagni](https://github.com/fluffypony), un des membre de l'équipe Monero. Cette solution est moins sûre, car sans support d'un wallet hardware comme le [LedgerWallet](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT), vous devrez entrer votre clé privée dans le navigateur à chaque transaction. Donc si ce site, votre navigateur ou votre ordinateur sont compromis, vous perdez tout.

Cependant, [les dernières informations](https://www.usethebitcoin.com/monero-is-being-tested-in-ledger-wallet-it-could-soon-be-fully-integrated/) montrent que le développement pour Ledger avance bien et devrait être bientôt disponible. 

![mymonero.png](https://steemitimages.com/DQmWsVcbvUC6bEuuhUMtdKp84KTgmA8rTVZNzW8hSLkjYbE/mymonero.png)

## Monerov et autres concurrents

Un fork de Monero a été annoncé pour la fin du mois. [D'après différentes analyses](https://serhack.me/articles/introduction-to-monerov-and-its-inherent-risks), ce fork semble être une attaque sophistiquée pouvant mettre en péril votre portefeuille et affaiblir l'anonymat des transactions. Ajoutons à cela que le code source du logiciel utilisé est fermé et invérifiable, que l'équipe se réserve 5% des tokens, et vous avez tous les ingrédients d'une arnaque.

Il est donc **vivement recommandé** de ne pas toucher à Monerov.

[Aucune autre monnaie majeure](https://gist.github.com/loryhuz/1d9d31eb76048a41a5095a2e99d7b77f) n'apporte les bénéfices décrits ci dessus : 

* **Verge (XVG)** protège uniquement l'identité de l'émetteur en passant par le réseau Tor ; 
* **Dash (DASH)** et **Zcash (ZEC)** supportent les transaction privées, mais de manière optionelle. On peut donc analyser le trafic.


## Mon avis ?

Le Monero est un beau projet, avec une très bonne équipe, une vision et une [roadmap claire](https://getmonero.org/resources/roadmap/). Elle n'est par exemple pas conçue pour proposer des smart-contracts comme ETH, mais pour rester une monnaie solide et fongible. Elle est l'unique option pour tous les acteurs qui ont besoin de protection dans leur transactions et c'est la seule monnaie qui peut luter contre les régulations et les interdictions.

Depuis quelques jours, le Monero est en chute libre, comme la totalité des crypto-monnaies. Actuellement, son cours est d'environ $183 / 0.024 BTC. 

L'objectif ici étant l'investissement long terme, je croise les doigts pour que le support du Ledger arrive assez tôt pour profiter de la baisse et remplir 15% de mon portefeuille.

![cap.png](https://steemitimages.com/DQmR7Cea5QL44Lj2ZLUCq1uJoYssBesAqLBYs63zczt5RRr/cap.png)
