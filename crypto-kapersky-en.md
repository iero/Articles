After writing a [post](https://steemit.com/crypto/@iero/what-is-a-ledger-wallet-and-why-do-you-need-one-now) describing the the Ledger Wallet Nano S, I came across two new products manufactured by **Kapersky Labs**, the well-known antivirus editor: [Ballet and Securator](https://wallet.kaspersky.com/).

![kapersky.png](https://steemitimages.com/DQmSvCAF78GPWU8NqQMaAPetVs2ayPR1XK7pG9jyuzPQMve/kapersky.png)

Before going further, if you want to understand the interest and the operation of a hardware wallet, and why it is absolutely necessary to have one to secure its cryptos, [read my article on the ledger](https://steemit.com/crypto/@iero/what-is-a-ledger-wallet-and-why-do-you-need-one-now).

## The devices

As the picture above shows, both devices look like old USB keys. The **Ballet** is the simplest one and costs $25. The **Securator** costs four times this price ($99), is slightly larger, with a screen and a lightning (iPhone) plug.

The design presented here is perhaps not the final one, but this is what we can see:

* Both are designed with an old-school soldered USB socket (as on old USB keys). You will need an extra adapter to use it on recent machines equipped with USB-C;
* There is no hole, so you can not use a necklace/cord (very useful to not lose the device)
* Microcontroller used looks classic, and equivalent to *ST31/STM32*. If they had something better (as the *CC EAL5+* certification of the Ledger) they would have specified it here.
* They have planned (but not developed yet as we can see on the the poor quality screenshots) to provide an iOS application to use the device from an iPhone (and surely Android too) by NFC wireless communication or direct lightning (with **Securator**). As [Apple Core NFC is not very open yet](https://medium.com/@vinceyuan/reading-and-parsing-nfc-tag-on-ios-11-60f4bc7a11ea), I don't think that Kapersky will be able to use wireless connection with Apple phones. Which would mean that only the 'luxury' version of devices would be compatible with an iPhone.
* There is no mention of Mac, Linux or Windows application, nor compatibility with [MyCrypto] (https://www.mycrypto.com). Do we need to use a Kapersky proprietary instance to perform transactions? I'm afraid we do.

The Kapersky support **few coins** compared to the ledger, but **the main ones are here**: Bitcoin, Bitcoin Cash, Ethereum, Classic Ethereum, Litecoin, Dash, Zcash and Ripple. They plan to add Bitcoin Gold, Monero and Dogecoin.

![Hain.png](https://steemitimages.com/DQmY3zbC1uT8jPwtsBt4GAUDytauhbRtp5GV5NvTSMsZjZN/hain.png)

Finally, there is a proposal to subscribe to "blockvault", a premium service (billed $30 per year) to make an "offline" copy of the device. There are few details on this option, but if it means to copy the private key (the famous 24 words passphrase) at Kapersky facilieies, it's a **very bad idea from a security point of view** . The best (only) way to secure this seed is to write it in a safe or use exotic things such as [steganography](https://en.wikipedia.org/wiki/Steganography). **Do not trust any third party player to store your key**!

## My opinion

Like [french Archos device](https://www.numerama.com/tech/331640-cryptomonnaies-archos-a-t-it-the-technical-materials-and-materials-of-the-right-to-leave.html ), Kapersky uses its brand to sell a new product and use the cryptocurrencies buzz: They say that they offer the **first** device created by *professionals in cybersecurity*, but [Ledger](https://www.ledgerwallet.com/) or [Trezor](https://trezor.io/) teams worked exclusively on this topic for several years, so I consider them as professionals too.

Kapersky labs has been the subject of many controversies in recent months and accused of [spying](https://www.tomsguide.com/us/is-kaspersky-safe,news-25983.html) for the Russian government. [Their products have been banned by law](https://www.reuters.com/article/us-usa-cyber-kaspersky/trump-signs-into-law-us-government-ban-on-kaspersky-lab-software-idUSKBN1E62V4) within the US government, and although they have very good engineers, this company has lost the trust of many users.
Their *BlockVault* proposal seems dangerous to me and does not provide enough information to prove anything in term of security.

After long years of calm, [security flaws have been found on Ledger devices](https://cointelegraph.com/news/teenager-who-hacked-ledger-hardware-wallet-says-devices-still-vulnerable-devs-deny) last week, but [the team has an excellent and very transparent communication](https://www.ledger.fr/2018/03/20/firmware-1-4-deep-dive-security-fixes/) and they published a fix very quickly. They also have a [very aggressive bug bounty policy](https://www.ledger.fr/bounty-program/).

All this gives us an important **guarantee of trust**, and it is clear that today the [Ledger](https://www.ledgerwallet.com/r/0b93?path=/products/ledger-nano-s&tracker=STEEMIT) is still the best choice to protect your Cryptos, and nothing justifies, at this stage, to buy a Kapersky device.