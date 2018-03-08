# Ledger Wallet : Comment ca marche ?

![Ledger-Wallet-Ledger-Nano-S-Cryptocurrency-hardware-wallet.png](https://steemitimages.com/DQmRnsJ4gDq5WekrYnAc8JFTvneTG4kWKoRfbNQjKRwCsSA/Ledger-Wallet-Ledger-Nano-S-Cryptocurrency-hardware-wallet.png)

Vos avoirs (BTC, ETH, etc) sont définis par deux informations : une clé publique et une clé privée. Pour faire très simple :
* la clé publique permet de recevoir des fonds (vous pouvez la partager sans problème)
* la clé privée permet d’envoyer des fonds. Il faut donc la **protéger pour pas perdre votre argent.**

Un portefeuille (wallet) est simplement une manière de stocker votre clé privée. Il y plusieurs manières de faire cela :
* la mettre sur un *portefeuille en ligne* : c’est simple mais le site peut se faire hacker ou même partir avec vos fonds. Il n’y a pas pire comme solution.
* la stocker dans un *fichier local* sur votre ordinateur et utiliser un portefeuille local. Si vous vous faites pirater, ou que vous perdez le fichier, c’est pareil, vous perdez tout. C’est à vous de faire vos sauvegardes, et ca ne sera utilisable que sur un seul appareil.
* la mettre dans un *gestionnaire de mots de passe*, de type 1password. C’est un bon compromis en attendant d’avoir un ledger !
* l’écrire sur un *papier* et la mettre dans un coffre fort. Plutôt sûr, mais pas super pratique.

## Alors, le ledger, c’est quoi ?

Le [ledger](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT) est un petit boitier qui se branche en USB sur votre ordinateur. Son rôle est de contenir les clés privées de vos portefeuilles et **elles ne sortiront jamais de ce boitier.**

Développé par une société Française, le ledger est rapidement devenu la référence sur le marché mondial. Il supporte une [vingtaine de monnaies](https://www.ledgerwallet.com/cryptocurrencies), dont les classiques BTC, ETH, LTC ou encore NEO. Par encore de [Cardano (ADA)](http://blocktribune.com/blockchain-firm-cardano-integrate-ledger-hardware-wallet/) ou de [Monero (XMR)](https://www.reddit.com/r/Monero/comments/7zez0g/ledger_hardware_wallet_monero_integration_some/), mais l’ajout de celles-ci est en cours. A noter, qu’il est possible de stocker les tokens dérivés de l’ETH *ERC20* souvent distribués par les ICO.

![1_-PocRvOF-EN-Sn0xY8S8qQ.png](https://steemitimages.com/DQmdeNSwseJVdUFYnJKJtz8wJkfsR49DwMz1TxCoosgeg5W/1_-PocRvOF-EN-Sn0xY8S8qQ.png)

Son seul réel concurrent, le Trezor, qui a été le premier sur le marché, [supporte beaucoup moins de cryptos et est plus cher](https://blockonomi.com/trezor-vs-ledger/).

Par rapport à de nouveaux concurrents, comme l’[archos safe-T](https://www.numerama.com/tech/331640-cryptomonnaies-archos-a-t-il-les-moyens-techniques-et-materiels-de-se-rever-en-ledger.html), le ledger est un produit sérieux avec un **microprocesseur sécurisé dédié** (*architecture dual chip ST31/STM32, mais certifié CC EAL5+*) par STMicroelectronics.

**Surtout, ne tombez pas dans le panneau, achetez un [vrai ledger](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT).**

## Quand l’utiliser ?

Un ordre de grandeur : Si vous détenez plus d’un demi mois de salaire en crypto-monnaies, il devient indispensable d’y stocker ses portefeuilles les plus importants. C’est ce qu’on appelle le *‘cold storage’*.

Le ledger coute un peu moins de 100€.. à vous de voir s’il vaut mieux perdre cette somme ou vos cryptos !

Pour les traders, il est conseillé de ne pas stocker beaucoup d’avoirs sur les exchanges (binance, kucoin, bitmex, etc), car différents piratages ont deja eu lieu ([MtGox](https://cryptoactu.com/dossier/de-mtgox-a-btc-e-chronique-cybercrime-plus-rocambolesque-de-lhistoire/), [Bitgrail](https://techcrunch.com/2018/02/12/bitgrail-hack-nano/)) et les utilisateurs ont tout perdu.

Il est très simple de transférer des fonds entre exchanges et ledgers. En plus, pour certaines monnaies (comme le NEO), le transfert est immédiat et gratuit. De mon coté, je ne met jamais plus de 10% de mes fonds sur des exchanges, et je garde le reste sur mon ledger.

## Comment ca marche ?

Par mesure de sécurité, il faut toujours acheter un Ledger neuf, [depuis le site du constructeur](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT). Ne passez pas par les sites d’annonces de particuliers, plusieurs cas d’arnaques assez sophistiquées ont été recensés, et le gain n’en vaut pas la chandelle.

Une fois reçu, il faut suivre la [documentation du site](https://www.ledgerwallet.com/products/ledger-nano-s) (et seulement celle là) : Créer une phrase de 24 mots, la noter sur une feuille et garder cette feuille en lieu sûr (coffre fort), et un code PIN d’au moins 6 chiffres. Attention de ne pas utiliser le même code que votre smartphone.. et de ne jamais le tapper devant quelqu’un, car avec votre ledger et ce code, un voleur pourra réaliser des transactions.

![Non, ceci n'est pas mon seed](https://steemitimages.com/DQmetA6vBsJUvLnWwahAg3Wy6C9oCxxwMR6coFVCHGm1Crz/ledger-recovery-seed.png)

Après, il suffit de télécharger le [Ledger manager et des applis dédiées](https://www.ledgerwallet.com/apps/). Pour chaque crypto, il faut installer, à partir de ce manager, une application dédiée sur le ledger. Ensuite, vous pouvez utiliser une application sur votre ordinateur comme [Ledger BTC](https://www.ledgerwallet.com/apps/bitcoin), [Ledger Ethereum](https://www.ledgerwallet.com/apps/ethereum) ou [Neon Wallet pour le NEO](https://github.com/CityOfZion/neon-wallet/releases) ([Procédure complète NEO](https://support.ledgerwallet.com/hc/en-us/articles/115005530425-How-to-install-and-use-Neo-NEO-)). Vous pouvez aussi utiliser [MyCrypto](https://mycrypto.com/) ([le successeur de MyEtherWallet](https://journalducoin.com/ethereum/fork-myetherwallet-mycrypto-suivre/)) en toute sécurité, vos transactions se faisant toujours depuis le ledger. Pour tout cela, la [documentation](https://www.ledgerwallet.com/apps) est très bien faite, et vous pourrez configurer tout ca très simplement.

## Et si ca ne marche plus ?

Si vous perdez le ledger, vous ne perdez pas vos cryptos ! Il faut en racheter un, rentrer vos 24 mots privés et c’est reparti. Quelle est cette magie ? C’est simple, vos clés privées [sont en fait dérivées de cette graine de 24 mots](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki), c’est pour ca qu’il faut la stocker en lieu sûr ! Si vous ne voulez pas en racheter un, [vous pouvez aussi extraire vos clés privées](https://support.ledgerwallet.com/hc/en-us/articles/115005197905-Restoring-your-Ethers-ETH-or-ETC-without-a-Ledger-Nano-S) à partir de la graine, mais ce n'est pas le plus facile à faire.

## C’est parti, j’en veux un !

Pour acheter un [ledger, c’est par ici sur le site de Ledger](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT) (c’est mon lien referral, n’hésitez pas) ! Je vous conseille le Nano S qui est super pratique et moins cher que l’autre modèle.

Pour ceux qui ont un ordinateur récent avec des ports USB-C, comme un macbook pro, pensez à commander en même temps un ‘cable court usb-c micro-b’ (environ 20cm) sur Amazon ou autre.

### @iero

Si cet article vous a été utile, vous pouvez [acheter un ledger en utilisant mon lien referral](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT). Ca ne vous coute pas plus cher, et je recevrai un petit pourcentage de votre achat (genre 5€)