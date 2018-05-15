Sur un fond de *Scream my name de Jingle Punks*, cette session de la [fameuse conférence pour les développeurs](https://events.google.com/io/) se déroulait à quelques kilomètres du siège de Google, au Shoreline Amphitheatre de Mountain View.

![google io.png](https://gateway.ipfs.io/ipfs/QmeEF1F6A3BfFtzF8m1BdhGCgNKbWHw8LHHiVKxtFu8naP)

Trois jours de sessions (keynotes), de zones à thèmes (sandbox) et d'ateliers (codelabs, office hours) avec des milliers de développeurs sur un grand terrain, parfaitement couvert par le wifi.

Une grande partie des annonces et [des sessions](https://events.google.com/io/schedule) de cette année étaient dédiées à Google Cloud et plus particulièrement au **Machine Learning** (#ml) sous toutes ses applications (**sémantique, d'images, audio, iot, assistant**). Ces trois jours montrent que l'intelligence artificielle (#ia) est clairement une priorité pour Google, et qu'ils continuent d'investir massivement sur cette technologie.

D'autres publications [ont présenté les générales](https://www.blog.google/topics/developers/all-io18-announcements/) autour du *bien être*, d'*Android P* ou des améliorations dans les *plateformes de dévelopement*. Je me focalise ici sur la partie **ML**. 

![IMG_5409.jpg](https://gateway.ipfs.io/ipfs/QmWeQLVQE7sgb5y83HWfVprdXiwCFdnHHGD2HL9piXKjcV)

## Sémantique : Smart Compose et Google News

La keynote principale a débuté par une [présentation impressionante](https://www.blog.google/products/gmail/subject-write-emails-faster-smart-compose-gmail/) du machine learning appliquée à Gmail : à partir du sujet et du destinataire, le modèle est capable de suggérer des phrases entières. Au fur et à mesure que l'utilisateur tape le mail, le contenu est pris en compte, les propositions s'affinent, et le résultat est impressionnant de pertinence.

![smartcompose](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_images/Smart-compose_Taco_Tuesday.gif)

En dehors de gagner du temps en faisant des mails plus rapidement, cette **technologie peut surtout être adaptée à d'autres domaines**, pour suggérer par exemple :

* des réponses aux **messages** quand on ne peut pas répondre (en voiture par exemple)
* des phrases dans la rédaction d'un **rapport**
* des morceaux de **code** dans un développement
* et finalement n'importe quel contenu textuel

Toujours dans le domaine du Natural Language Processing (#nlp), Google [lance un nouveau service de news](https://www.blog.google/products/news/new-google-news-ai-meets-human-intelligence/). Basé sur des sources sélectionnées parmis des journalistes reconnus, le système est capable de comprendre, classer, dédoublonner, et synthétiser les nouvelles par thèmes pour les présenter aux utilisateurs sous forme d'un *executive briefing*. Si ceux-ci veulent aller plus loin dans la compréhension d'un sujet, [Google présentera un dossier](https://news.google.com/about/) plus complet, fabriqué automatiquement à partir de plusieurs sources (dont Youtube).

![google news](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_images/gnews_blog_fullCoverage.gif)

Google semble s'inspirer d'[Apple news](https://www.apple.com/news/),
 qui n'a jamais vraiment décollé, en pariant sur un fil *simplifié* créé avec un moteur de machine learning différent. Est-ce suffisant pour faire la différence et s'imposer comme une référence ?

Au delà de ce pari, cela montre que de **nombreuses briques sémantiques sont prêtes** à être utilisées : extraction d'entités, de relations, construction de graphes de connaissances, dédoublonnage, sélection.

## Images, vidéo et capteurs : Google photos et Waymo

Dans Google Image, de nouvelles fonctions sont poussées au bon moment à l'utilisateur via un **assistant intelligent**. Par exemple, le système peut proposer, après avoir analysé l'image, d'augmenter le contraste, de mettre le fond en noir et blanc, ou même de la re-colorer. Il n'y a rien de plus à faire que d'accepter la proposition. La rupture n'est pas ici dans les algorithmes, car de nombreuses sociétés sont capables de proposer ces outils. Mais le système d'agent intelligent proposant, **au bon moment** le bon filtre à appliquer peut faire la différence parmis les concurrents. Cette méthode prédictive peut être appliquée dans des domaines connexes (sélection de la bonne couleur, affichage du bon menu) et proposer des interfaces plus simples et conviviales (#ux)

![google images](https://gateway.ipfs.io/ipfs/QmXjm6fzthVsUECdnHLoF6r89ErTk1NqfE6B4deMFUbD5y)

La société de voitures autonomes du groupe Alphabet, Waymo, a montré ses dernières avancées en **analyse de flux vidéo et multi-capteurs**, avec par exemple les résultats de machine learning pour améliorer la compréhension d'un [environment sous la neige](https://medium.com/waymo/google-i-o-recap-turning-self-driving-cars-from-science-fiction-into-reality-with-the-help-of-ai-89dded40c63).

Ses voitures autonomes tournent déjà en boucle à Phoenix en Arizona avec plusieurs familles pilotes et ils prévoient une ouverture de ce service Q4 2018. Des camions autonomes sont aussi actuellement en test.

![IMG_5549.jpg](https://gateway.ipfs.io/ipfs/Qmb3AYxmssqduTeSbiG1hELtkohTKDos3hSZmGzPxbxnfz)

Le deep learning est largement utilisé pour prendre les décisions en fonction des informations provenant des différents capteurs. La course aux données est bien sûr un pré-requis, mais la société qui aura les meilleurs modèles de prédiction sera la première à pouvoir mettre massivement ses voitures sur la route et à prendre de l'avance technologique sur les autres, comme SpaceX face à Blue Origin. Le défi est actuellement lancé entre Tesla, Uber et Waymo.

## Vocal : Musique, Google Assistant et Duplex

De nombreux projets autour de la voix ou de la musique sont en cours, comme [N-Synth](https://nsynthsuper.withgoogle.com/), un synthétiseur permettant de créer de nouveaux instruments, avec leur sonorité, à partir de machine learning appliqué à des instruments de musique existants. Le projet [Magenta](https://magenta.tensorflow.org/) qui permet, entre autres, de compléter une partition de musique, a eu le droit à son stand et à une présentation pleinière. **Ces projets restent cependant à un niveau hobby/recherche**, s'adressant au segment particulier des professionnels de la musique et ne semblent pas encore avoir trouvé un business model général.

Mais dans le domaine vocal, Google met surtout du poids sur son assistant *OK Google*. En dehors des fonctionnalités de base, qui sont [comparables à celles d'Alexa d'Amazon](http://www.zdnet.fr/actualites/google-home-vs-amazon-alexa-qui-est-le-plus-malin-maj-39855788.htm), le machine learning est maintenant aussi utilisé pour affiner les voix, les intonnations et les transitions afin de les rendre plus naturelles avec le modèle [WaveNet](https://cloud.google.com/text-to-speech/docs/wavenet).

Mais le plus impressionant fut la démonstration de Google Duplex, un assistant capable de tenir une conversation pour prendre un rendez-vous au restaurant ou chez le coiffeur. L'IA a sû s'adapter pour prendre en compte les contraintes du coiffeur ou les questions étonnantes du restaurant.

https://youtu.be/D5VN56jQMWM?t=45s

On voit donc les prémices d'un agent conversationnel avancé, qui va devenir petit à petit beaucoup plus autonome dans les discussions. On peut rêver d'un agent Google qu'on utilisera pour interagir avec des humains non-connectés et lui faire réaliser toutes les taches vocales pénibles (prises de rendez vous, commande d'un produit, récupération d'information), mais on peut trouver des usages plus sophistiqués comme **négocier un prix**, ou plus inquiétantes comme l'**automatisation du social engineering** (arnaques et hameçonnage à grande échelle) Les possibilités sont infinies ! Je ne serais d'ailleurs pas étonné par exemple que Google (ou d'autres entreprises) utilise cette technologie pour améliorer à faible coût ses services en demandant par exemple par téléphone à tous les commerces leurs horaires d'ouvertures, ou les prix de leurs services.

## Hardware : TPU et IOT

Grande nouveauté hardware : la nouvelle génération des Tensor Processing Units (TPU) est annoncée :

* 2015 : TPU v1, 92 teraops , inference only
* 2017 : Cloud TPU (v2), 180 teraflops, training et inference
* 2017 : TPU Pod, 11. petaflops
* **2018 : TPU v3 : Plus de 100 petaflops**

Ces nouveaux processeurs sont huit fois plus performants que les fameux TPUv2 pod actuellement proposés sur GCP. Ce qui fait encore chuter le temps de calcul et donc le prix des entrainements des algorithmes de machine learning.

![IMG_5429.jpg](https://gateway.ipfs.io/ipfs/QmckumTFgLngQQ2Ef59UsYUzeavzRH6Nxckci5PrDSwAUu)

Sur Android P, le machine learning est appliqué à la gestion de la batterie. Android essayera de prédire quelles seront les prochaines applications utilisées et mettra en veille celles n'ayant pas besoin d'être redémarrées. Même chose pour adapter la luminosité à l'environnement et à l'usage. Ils annoncent un gain de 30% de batterie.. de quoi faire une journée sur une seule charge ?

Google se met aussi à l'internet des objets (#IOT) et au Do It Yourself (#DIY) en proposant des [kits AIY (Artificial Intelligence Yourself](https://aiyprojects.withgoogle.com) comprenant une partie hardware à base de Raspberry Pi Zero et une partie software sur Raspian et GCP. Il y a différents exemples fournis, comme un module de reconnaissance d'objets ou d'émotions utilisant les services IA de GCP.

Plusieurs autres projets ont été présentés, utilisant Tensorflow Lite, comme les voitures autonomes mignatures [Donkey Cars](http://www.donkeycar.com/), de fausses fleurs qui réagissent aux sourires ou les classiques détecteurs de pommes et bananes.

Dans les goodies que les participants ont reçu, il y avait d'ailleurs un [kit Android Things 1.0](https://developer.android.com/things/) basé sur un Pico i.MX7Dual et contenant une caméra, ainsi qu'un écran tactile. Ce kit est très complet, et c'est une très bonne base pour construire de petits prototypes, comme un [module de reconnaissance d'objets avec TensorflowLite](https://androidthings.withgoogle.com/#!/samples/sample-tensorflow-imageclassifier) ou une [station météo](https://androidthings.withgoogle.com/#!/samples/weatherstation).

![inventory.png](https://gateway.ipfs.io/ipfs/QmURQ1aXqv9npuME2Z2A6qbveMmkzht1wzhvjkV2T81Dmk)
  
## Coté fun et développement

Tout l'amphithéâtre a joué pendant une bonne demi-heure avec la suite de Quickdraw : [Worlddraw](https://worlddraw.withgoogle.com/explore). Le principe est de dessiner un objet que Google reconnaitra et insérera en 3D sur une carte. Rien de révolutionnaire depuis l'annonce de Quickdraw il y a deux ans, et [le milliard de doodle dessinés depuis](https://towardsdatascience.com/quick-draw-the-worlds-largest-doodle-dataset-823c22ffce6b) mais le jeu multi-joueurs était amusant.

![google world draw.png](https://gateway.ipfs.io/ipfs/QmdSVBuHYtw6s8F8igzudKvR5iZuCbUFvwVc3SBx87Bkzb)

Une belle session de Martin Gorner sur l'utilisation de Tensorflow pour jouer à Pong avec les [étapes expliquées pas à pas](https://github.com/GoogleCloudPlatform/tensorflow-without-a-phd). Fidèle à la philosophie OpenSource, ce code est complètement disponible pour servir d'exemple à d'autres usages d'apprentissage non-supervisé basé sur une analyse de pixels.

En plus des nombreuses sessions encourageant à l'utilisation de Tensorflow Lite sur les appareils mobiles, l'annonce de [ML Kit](https://developers.googleblog.com/2018/05/introducing-ml-kit.html), le nouveau concurrent d'Apple CoreML, va faciliter les développements ML sur Android et même iOS (via Firebase).

# Mot de la fin

Peu de choses autour d'autres domaines, comme le développement d'applications, la réalité virtuelle/augmentée ou la blockchain. Cependant, Google a fait du chemin ces dernières années et montre pendant cette conférence que le machine learning n'est plus une discipline obscure, mais la réponse à de nombreux usages d'aujourd'hui et de challenges de demaon. Ils en appliquent les résultats dans tous les domaines : images, texte, vidéo, voix, matériel et de nombreuses ressources sont à la disposition des entreprises ou des particuliers pour qu'ils s'approprient cette technologie à travers GCP ou Android. Comme disent régulièrement les keynote speakers :

> J'ai vraiment hate de voir tout ce que vous allez créer de génial avec cette technologie

Vivement le mois prochain pour voir la réponse d'Apple [pendant la WWDC](https://developer.apple.com/wwdc/), puis novembre pour celle d'Amazon [pendant AWS:reinvent](https://reinvent.awsevents.com/) qui, j'espère, feront monter la barre d'un cran encore !
