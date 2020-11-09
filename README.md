Awesome lnurl [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) <img src="https://i.imgur.com/wNtVhj3.png" width="200" align="right" alt="./jq">
========================================================================

A curated list of awesome things related to the **lnurl** super-protocol for interaction between [Lightning](https://github.com/lightningnetwork/lightning-rfc) wallets and third-party services.

* [Awesome **lnurl**](#awesome-lnurl)
  * [Documentation](#documentation)
  * [Services](#services)
  * [Wallets](#wallets)
  * [Libraries](#libraries)
  * [Tools](#tools)
  * [Contribute](#contribute)
  * [License](#license)

----


Documentation
------------------------------------------------------------------------

_Readings about **lnurl**_.

* [The spec](https://github.com/btcontract/lnurl-rfc) &ndash; The confusing, but honest, **lnurl** spec.
* [lnurl-auth explained](https://xn--57h.bigsun.xyz/lnurl-auth.html) &ndash; Everything you always wanted
* [lnurl-withdraw flow](https://⚡️.bigsun.xyz/lnurl-withdraw-flow.txt) &ndash; One of those incomprehensible program action-data flows detailing how **lnurl-withdraw** takes place.
* [lnurl-pay flow](https://⚡️.bigsun.xyz/lnurl-pay-flow.txt) &ndash; Same as above, but for **lnurl-pay* (doesn't include all features).
* [Coindesk article](https://www.coindesk.com/bitcoin-wallets-are-adopting-this-tech-to-simplify-lightning-payments) &ndash; An honest report on **lnurl**.
* [Beyond Coffee: Bitcoin for Every Day Use with LNURL](https://degreesofzero.com/article/beyond-coffee-bitcoin-for-every-day-use-with-lnurl.html) &ndash; An insightful article with explanations and use cases.


Services
------------------------------------------------------------------------

_Apps and services supporting **lnurl** in the wild_.

### lnurl-pay

* [Bitrefill](https://bitrefill.com/) &ndash; Allows funding your account with **lnurl**.
* [lntorub](https://vds.sw4me.com/rulnurl/)	&ndash; Build reusable URLs that allow you to recharge Russian transport tickets, phones, send money to Russian debit cards and recharge Skype globally.
* [lnbits](https://lnbits.org/) &ndash; The LNURLp plugin allows anyone to generate **lnurl** payment codes and dispatch webhooks whenever a new payment comes in.
* [Lightning Gifts](https://lightning.gifts/) &ndash; Create gifts without leaving your wallet by playing and replaying the basic gift **lnurl**.
* [Etleneum](https://etleneum.com/) &ndash; For all reusable method calls, with or without a fixed number of satoshis in them, you can grab an **lnurl** at the main contract page and replay it from your wallet later.
* [Blixt's lnurl-pay chat](https://chat.blixtwallet.com/) &ndash; A simple chat you have to pay 10 satoshis to send an anonymous message directly from your wallet (the interface is just a QR code) as a proof-of-concept for lnurl-pay comments.
* [tip.bigsun.xyz](https://tip.bigsun.xyz) &ndash; Static donation **lnurls** that send money directly to your node, noncustodially. Ideal for street musicians.
* [@lntxbot](https://t.me/lntxbot) &ndash; `https://lntxbot.bigsun.xyz/@telegramusername` allows you to send money to anyone using a fixed **lnurl**. It can be printed and shared at will. It's basically an old-style address.
* [zbd.gg](https://zbd.gg/) &ndash; Static **lnurl pay** QR codes for users of ZEBEDEE Wallet to accept payments and messages.
* [coinos](https://coinos.io/) &ndash; Allows you to fund your account with an **lnurl**.

### lnurl-auth

* [LNMarkets](https://lnmarkets.com/) &ndash; **lnurl** is a private login option.
* [Etleneum](https://etleneum.com/) &ndash; The only supported login method is **lnurl**.
* [Wheel of Fortune](https://fortune.lngames.net) &ndash; Login with **lnurl** Instead of manually saving your key.
* [coinos](https://coinos.io/) &ndash; Allows you to add multiple _linking keys_ to the same account.

### lnurl-withdraw

* A big collection of services allow you to withdraw your balances with **lnurl**: [Etleneum](https://etleneum.com/), [Paywall](https://paywall.link), [Kriptode](https://kriptode.com/), [lngames.net](https://lngames.net/), [LightningScratchAnd.win](https://lightningscratchand.win/), [Lightning Gifts](https://lightning.gifts/), [LNMarkets](https://lnmarkets.com/), [Stekking](https://stekking.com), [Microlancer](https://microlancer.io/).
* And also exchanges: [GraafOne](https://www.graaf.one/) on Canada and [SouthXchange](https://www.southxchange.com/) on Argentina.
* [ZEBEDEE](https://documentation.zebedee.io/) &ndash; The REST API for game developers and [Unity SDK](https://github.com/zebedeeio/unity-sdk) automatically generates **lnurl** links that allow players to easily withdraw sats from the game.
* [Bitcoin Bounce](https://thndr.games/) &ndash; Play for free and win satoshi prizes. **lnurl** is the only way to redeem.
* [LNPay.co](https://lnpay.co) &ndash; Provides static **lnurl** rechargeable faucets you can print, email or easily embed!
* [@arcbtc's TheFossa](https://twitter.com/BTCSocialist/status/1176206194333147136) &ndash; A DIY ATM machine that eats coins and spits out sats.
* [coinos](https://coinos.io/) &ndash; Allows you to issue **lnurl** vouchers.
* [lnbits](https://lnbits.org/) &ndash; The LNURLw plugin allows anyone to generate **lnurl** vouchers.
* [LightningCashback](https://twitter.com/21isenough/status/1193631492603293698) &ndash; A POS system that prints **lnurl** QR codes containing your change in receipts (fiat onramp?).
* [@21isenough's LightningATM](https://twitter.com/21isenough/status/1194963700110770176) &ndash; A DIY ATM machine that eats coins and spits out sats.
* [Bleskomat](https://github.com/samotari/bleskomat) &ndash; The offline Lightning Network ATM - device source code, lnurl server implementation, and build instructions included.
* [@lntxbot](https://t.me/lntxbot) &ndash; You can extract your balance from the Telegram bot to another wallet with **lnurl**, or even share withdraw codes so you can physically pay friends.
* [LNURLProxyAPI](https://github.com/21isenough/LNURLProxyAPI) &ndash; Allows you to issue noncustodial **lnurls** from your own home node, wait until someone tries to redeem them and pay the invoice. Like lightning.gifts, but noncustodial.
* [Rewards to Bitcoin](https://play.google.com/store/apps/details?id=com.pseudozach.rewardstobitcoin) &ndash; Android app that lets you cash out Play Store balance with **lnurl**

### lnurl-channel

* [LNBIG](https://lnbig.com/) &ndash; Get free inbound channels on your mobile wallet from this mysterious entity.
* [Bitrefill's Thor](https://www.bitrefill.com/thor) &ndash; Buy a reliable incoming channel from this super liquid node, or get a turbo channel from which you can spend immediately.
* [bifrost](https://github.com/takinbo/bifrost) &ndash; A self-hosted **lnurl**-powered invite-based channel-opening service.
* [lnch-vekslak](https://github.com/Kixunil/lnch-vekslak) &ndash; Your self-hosted Thor. Allows you to sell or open channels with people in the streets (make sure to read and edit the code before using or you'll pay a high price).


Wallets
------------------------------------------------------------------------

_Some wallets that support **lnurl**_.

| Wallet                                                   | fallback¹ | withdraw | pay   | auth  | channel |
| ---:                                                     | :---:     | :---:    | :---  | :---: | :---:   |
| [BLW](https://lightning-wallet.com/)                     | ☑️         | ☑️        | ☑️     | ☑️     | ☑️       |
| [Blixt](https://github.com/hsjoberg/blixt-wallet)        |           | ☑️        | ☑️ 💬  | ☑️     | ☑️       |
| [BlueWallet](https://bluewallet.io/)                     |           | ☑️        | ☑️     |       |         |
| [Breez](https://breez.technology/)                       |           | ☑️        |       |       | ☑️       |
| [coinos](https://coinos.io/)                             |           | ☑️        | ☑️     | ☑️     | ☑️       |
| [lnbits](https://lnbits.org/)                            | ☑️         | ☑️        | ☑️ 💬  |       |         |
| [@lntxbot](https://t.me/lntxbot)                         | ☑️         | ☑️        | ☑️ 💬  | ☑️     |         |
| [Phoenix](https://phoenix.acinq.co/)                     | ☑️         | ☑️        |       | ☑️     |         |
| [Shockwallet](https://shockwallet.app/)                  | ☑️         | ☑️        | ☑️     |       | ☑️       |
| [Wallet of Satoshi](https://www.walletofsatoshi.com/)    | ☑️         | ☑️        |       |       |         |
| [Zap-iOS](https://www.zaphq.io/)                         |           | ☑️        | ☑️     |       | ☑️       |
| [Zap-Android](https://www.zaphq.io/)                     | ☑️         | ☑️        | ☑️     |       | ☑️       |
| [Zeus](https://github.com/ZeusLN/zeus)                   | ☑️         | ☑️        | ☑️ 💬  |       |         |
| [ZEBEDEE](https://zbd.gg)                                | ☑️         | ☑️        | ☑️ 💬  |       |         |

*¹=the **fallback scheme** is defined on the first page of the [LNURL specifications](https://github.com/btcontract/lnurl-rfc#fallback-scheme). It allows to embed an bech32-encoded LNURL string into a normal Web-URL so that for example a LNURL QR code can be opened on every smartphone as a fallback with a normal web browser (if a specialised wallet app is not installed yet). Every LNURL supporting wallet should be able to parse such Web-URLs for bech32-encoded LNURL strings - it easy to implement and just requires a handfull of additional lines of code.*

Libraries
------------------------------------------------------------------------

_Integrate **lnurl** in projects and services_.

* [go-lnurl](https://github.com/fiatjaf/go-lnurl) &ndash; **lnurl** helper structs, encode/decode, verify signatures, misc helpers.
* [lnurl-node](https://github.com/chill117/lnurl-node) &ndash; CLI tool and **lnurl** server in Node.js.
* [passport-lnurl-auth](https://github.com/chill117/passport-lnurl-auth) &ndash; Passport strategy that uses lnurl-auth
* [js-lnurl](https://github.com/fiatjaf/js-lnurl) &ndash; Tools for adding **lnurl** support in a JavaScript wallet.
* [php-lnurl](https://github.com/tkijewski/php-lnurl) &ndash; Easy PHP encoding and decoding of bech32 **lnurl**s.
* [python-lnurl](https://github.com/python-ln/lnurl) &ndash; Tools for dealing with **lnurl** in Python.
* [lnurl-ruby](https://github.com/bumi/lnurl-ruby) &ndash; A gem that provides helpers to work with **lnurl** from Ruby.
* [lnurl-rust](https://github.com/edouardparis/rust-lnurl) &ndash; Rust helpers for **lnurl**.
* [lnurl.net](https://github.com/Horndev/lnurl.net) &ndash; Library for **lnurl** in C#. Provides lnurl-auth helpers.
* [dart_lnurl](https://github.com/bottlepay/dart_lnurl) &ndash; Library for **lnurl** in Dart.


Tools
------------------------------------------------------------------------

_Stuff for learning, using and playing with **lnurl**_.

* [lnurl codec](https://lnurl.bigsun.xyz/codec) &ndash; Easily encode and decode **lnurls**.
* [lnurl-toolbox](https://lnurl-toolbox.degreesofzero.com/) &ndash; A web interface with tools for testing and integrating **lnurl**.
* [SeedAuth](https://seedauth.etleneum.com/) &ndash; A JS app that allows you to login to **lnurl-auth** services using just a username and password.
* [lnurl playground](https://lnurl.bigsun.xyz/) &ndash; A simple tool that allows you to try and see how your wallet interacts with an **lnurl** server.
* [SeedAuthExtension](https://github.com/pseudozach/seedauthextension) &ndash; A Chrome & Firefox extension that allows you to login to **lnurl-auth** services using just a username and password.

Contribute
------------------------------------------------------------------------

Please contribute! Open an issue or a PR and we’ll discuss it or merge it. If
you’re opening a PR, please ensure all formatting is ok (if you’re in a hurry
just open an issue).


License
------------------------------------------------------------------------

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
