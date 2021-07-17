[![NPM](https://nodei.co/npm/utilia.png)](https://nodei.co/npm/utilia/)

# Utilia
 An NPM package for you to use on your Discord Bot or JavaScript projects! This is still however in development and countless of errors have been encountered, if you wish to help me add features, make a pull request at the github page!

## What's New?

### Added
- NitroChecking functions (Utilia.hasNitro(user: User))
## TODO

- Work on custom embed class

 ## Getting Started

 To get started, install the npm package by running the command below:

With NPM:

```shell
npm install --save utilia
```

With Yarn:

```shell
yarn add utilia
```

## Table of Contents

- [Captcha](##Captcha)
- [QRCode](##QRCode)
- [Api](##Api)
- [Utils](##Utils)

## Captcha

Generates a captcha value and an image

Example:

```js
const { Captcha } = require('utilia')

// New Captcha Client
const captcha = new Captcha()

// Outputs the value of the image
console.log(captcha.value)
```

## QRCode

```js
const { QRCode } = require('utilia')

// New QRCode Client
const qr = new QRCode({
    // Data - your url
    data: "owenpotent.xyz"
})

// Generate the QRCode link
const qrcode = qr.genQR()

// Outputs the qrcode link
console.log(qrcode)
```

## Api

```js
const { Api } = require('utilia')

const api = new Api()

const text = "Hello world"

api.encode(text).then((data) => {
    console.log(data) // Outputs binary code : '0100100001100101011011000110110001101111001000000111011101101111011100100110110001100100
})
```

## Utils

```js
const { Utils } = require('utilia')

const util = new Utils()

const textHi = "hash time"
const hash = util.createHash(textHi, "sha256")

console.log(hash) // Outputs hash: e624d76c1654e78cd3479aaeaec930a6f194ab349878201d645de8912fb8a4ca
```

# Additional Info

Utilia.Embedder - A custom but more cleaner embed feature highly inspired from the [discord.js](https://discord.js.org) MessageEmbed class.  
Utilia.hasNitro - Typescript support from the original feature by @thehackerboi69's [discord-premium-utils](https://www.npmjs.com/package/discord-premium-utils) dependency.  


# Links
- [Source Code](https://github.com/OwenPotent/utilia)

## More coming soon!