# libp2p-crypto-from-seed

## Install

```sh
yarn add https://github.com/kungfuflex/libp2p-crypto-from-seed
```

## Usage

```js
const { ethers } = require('ethers');
const randomValue = ethers.utils.hexlify(ethers.utils.randomBytes(32));

const { cryptoFromSeed } = require('libp2p-crypto-from-seed');

(async () => {
  const key = await cryptoFromSeed(randomValue);
  // construct peerId from crypto, or whatever libp2p stuff
})().catch((err) => console.error(err));

## Author

flex
