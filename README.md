# QRANoDe

## A quantum random number generator for node.js.
Gets N-length random numbers from the ANU Quantum Random Number Generator

See here for more info: https://anuquantumoptics.org/research-topics/qrng

[NPM Link](https://npmjs.com/package/qranode)


## Installation

`npm i qranode`

## Usage:

```js
const qranode = require('qranode')
// promise

qranode('uint8', 5) // get 5 numbers from 0 to 255
.then(console.log) // log the output
.catch(console.error) // or the errors, if any

// async/await

let numbers = await qranode('uint8', 5)

// you can even get hex!

qranode('hex16', 5, 2) // get 5 hex strings, each string consisting of 2 hex blocks between 0000 and ffff
```
