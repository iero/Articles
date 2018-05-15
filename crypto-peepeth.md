![peepeth.png](https://gateway.ipfs.io/ipfs/QmYXDsQCNJwKqeSx2fAcAtCK1cHgZghpZxbGZbUKnQzYp3)

Actuellement, le marché du micro-blogging, c'est à dire la communication à un large public (one to many) via du texte court se résume quasi-intégralement à un seul acteur : Twitter.

Twitter est centralisé, c'est à dire que cette société contrôle les conditions d'utilisation, [censure](http://www.lepoint.fr/high-tech-internet/twitter-interdit-a-son-tour-certaines-publicites-liees-aux-crypto-monnaies-26-03-2018-2205738_47.php) ce qui ne lui plait pas, [supprime](https://www.numerama.com/tech/343912-la-suspension-du-compte-bitcoin-sur-twitter-alimente-des-theories-du-complot.html) des comptes sans justification et finalement [une bonne partie](https://www.cnet.com/news/new-study-says-almost-15-percent-of-twitter-accounts-are-bots/) des utilisateurs sont en fait des bots.

Pour corriger tout cela, [Mastodon](https://joinmastodon.org/), un service alternatif de Micro-blogging, a été conçu de manière communautaire ([logiciel libre](https://github.com/tootsuite/mastodon)) et décentralisée (avec des instances, c'est à dire des serveurs à thèmes qui se connectent entre eux).

![screenshot_full.e8e4a020.png](https://gateway.ipfs.io/ipfs/Qmd93ZkjsyBizjqK24T8NiSzyDp73nHAPyPrwvGe4Qy2e5)

Cependant, même si l'idée est excellente, après avoir fait le buzz en avril 2017, puis passé le million d'utilisateurs en décembre 2017, Mastodon peine encore à convaincre. 

Les notions d'instances restent complexes à comprendre (Fil public local vs global) et les communautés semblent rester trop cloisonnées. Les utilisateurs sont encore principalement des geeks et/ou libristes et/ou anarchistes, et les utilisateurs non-spécialistes sont restés à l'écart.

Après avoir posté [près de 40 000 pouets](https://mamot.fr/@fabre_gregori) sur Mastodon et [plus de 45 000 tweets](https://twitter.com/gfabre_digital) sur Twitter, je trouve que Mastodon génère des interactions bien plus riches avec les utilisateurs (de vrais échanges et débats), mais le contenu y est infiniment plus pauvre.

![twitter vs mastodon.png](https://gateway.ipfs.io/ipfs/QmTFApbAN2rs1Zcee8uKz3M3Uy7i5oSHJDzUcPX2MWGYvg) 

Je reste donc sur Mastodon pour la qualité des échanges, mais je privilégie Twitter pour ma veille. Ce qui fait un ratio de 5% de temps passé sur Mastodon par rapport à Twitter.

##  C'est là que Peepeth rentre en course

Un nouveau service a été annoncé il y a quelques jours sur [Reddit](https://www.reddit.com/r/ethereum/comments/87k9iz/presenting_peepeth_a_decentralized_alternative_to/) : **Peepeth**

[Peepeth](https://peepeth.com) est un service de micro-blogging décentralisé, basé sur les dApps de la blockchain Ethereum.

Ce service est donc, par design, décentralisé, résistant à la censure et incorruptible (les messages sont gravés dans la blockchain). Si Twitter tombe ou que votre instance locale de Mastodon tombe, vous êtes déconnectés. Ici, si le client (frontend) qui donne accès à la blockchain tombe, il suffit d'en choisir un autre pour retrouver les mêmes informations.

A la différence des autres services, Peepeth n'est pas gratuit et financé par des bénévoles (Mastodon) ou par de la publicité (Twitter). Pour entretenir le réseau, chaque message envoyé coute une petite fraction de centimes en ethereum (payment par smart-contract).

On peut aussi remercier un utilisateur en envoyant un tip en ethereum (dont 10% sont prélevés par Peepeth). Chaque message posté est reposté automatiquement sur Twitter une fois que le compte est vérifié, et il y a des clients mobile. Les posts et images sont enregistrés sur [IPFS](https://fr.wikipedia.org/wiki/InterPlanetary_File_System).

Le frontend créé par l'auteur est sympathique et rapide :

![p.png](https://gateway.ipfs.io/ipfs/QmaqNWPN6d7pxC9Re1fvLDPAdAxmYPU6QXYtkveQq3tzJe)

Par contre, autant le projet semble séduisant, autant je me pose de sérieuses questions sur son avenir :

* Le **nom est clairement mauvais**, je vous laisse chercher la traduction de Pee ou Peep.
* Il ne s'adresse qu'aux **porteurs d'ethereum**, qui ne sont aujourd'hui qu'une minuscule partie du monde.
* Le système n'est **pas très pratique**, car il faut lier un compte Ethereum à Peepeth via un plugin de navigateur (Metamask).
* Il faudrait une **communauté avec une gouvernance** pour continuer le développement. D'ailleurs, je ne trouve pas le code source du backend.
* 10% d'un tip vont au projet, et je trouve ca vraiment élevé.

Donc pour l'instant je n'ajoute pas tout de suite ce nouvel outil à [ma panoplie](https://steemit.com/fr/@iero/communiquer-en-2018) mais je vais suivre le projet avec attention, et voir s'il décolle ou si d'autres prennent le relais en faisant évoluer l'idées !