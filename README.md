![](https://lemon.email/images/logo-blue.svg)
[![codecov](https://codecov.io/gh/Ami-Solution/amis-lemon/master/graph/badge.svg)](https://codecov.io/gh/Ami-Solution/amis-lemon)
[![Coverage Status](https://coveralls.io/repos/github/Ami-Solution/amis-lemon/badge.svg?branch=master)](https://coveralls.io/github/Ami-Solution/amis-lemon?branch=master)
[![Travis](https://travis-ci.org/Ami-Solution/amis-lemon.svg?branch=master)](https://travis-ci.org/Ami-Solution/amis-lemon)
[![Build status](https://ci.appveyor.com/api/projects/status/?svg=true)](https://ci.appveyor.com/project/Ami-Solution/amis-lemon)
[![CircleCI](https://circleci.com/gh/Ami-Solution/amis-lemon.svg?style=svg)](https://circleci.com/gh/Ami-Solution/amis-lemon)


# LemonMail DApp

[LemonMail DApp](https://ipfs.io/ipns/dapp.lemon.email/) is a completely decentralized version of [LemonMail](https://lemon.email), a security-focused email service. Functioning as a stand-alone version of LemonMail, the DApp consist entirely of front-end Javascript code that interacts with an Ethereum contract that serves as a back-end. All message content is end-to-end encrypted and stored on IPFS, a peer-to-peer storage network. The front-end code is open source and also hosted on IPFS (although you are free to deploy and run it anywhere you want). Utilizing decentralized technologies such as Ethereum and IPFS along with public key encryption ensures both platform stability and user privacy. No one can access other users' messages, tamper with the message content or take the service down - not even us!

This is a highly experimental software that aims to demonstrate that it is possible to achieve secure message exchange without trusted third-party. We encourage you to inspect the code and even deploy your own instance of the application and run it wherever you want - locally, on your own server or on IPFS. See below for instructions on how to build and deploy the code. Because we are still at an early testing stage, the Ethereum contract runs on a testnet. You will need a small amount of Kovan Ether in order to use the Dapp - get in touch and we'll be more than happy to send you some!

# Building and deployment

In order to build the application, run the following:

```
npm install
npm run production
cp -r public/web/dist/* publicIpfs
```

Then if you want to publish the application on IPFS, run:

```
ipfs add -r publicIpfs
```

You should receive the following hash: 

```
QmfJ856Hu6LCHo64eMrvnKPpqevAkB8aJ83o1cMrtt59KM
```

You can then access the app through an IPFS gateway, e.g. https://ipfs.io/ipfs/QmfJ856Hu6LCHo64eMrvnKPpqevAkB8aJ83o1cMrtt59KM

# The changelog

### Alpha 0.1 - 02.05.2017.

- Initial alpha release

