# Qubic Typescript Library

A TS Library to communicate with the Qubic Network.

## Usage
Install via NPM.

```bash
yarn add @qubic-lib/qubic-ts-library
```

### TS Examples

```ts
// import helper
import { QubicHelper } from 'qubic-ts-library/dist/qubicHelper'

// create an id Package with private/public key and human readable address
const id = await helper.createIdPackage("alsdjflasjfdlasdjflkasdjflasdjlkdjsf");
```

## Build a single JS File
```
yarn install
yarn webpack
```

## Node Sample Applications

### requestBalance.js
Test how to receive Balance from Network

Add the Ids to `const ids = ["AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"];` in file `test/requestBalance.js` and:

```bash
yarn install
tsc
node test/requestBalance.js
```

### sample-exchange.js
Ultry light weight sample of an exchange integration to Qubic.
It Can manage multiple users and to Deposits/Withdraws to one hot wallet.

> This Implemenation is meant for demo purposes only!

How to run?

```bash
yarn install
tsc
node test/sample-exchange.js
```

The Exchange initializes itsself. Start it and it will create a file `exchange.json`. There you can find the Seeds used. If you do tests, save them anywhere.

## Testing
Run tests with

```bash
yarn run test
```

## Publish
publish with.

```bash
yarn build
yarn publish --access public
```

## LICENSE
All Qubic Software is licensed unter the Anti Military License: https://github.com/qubic-network/license