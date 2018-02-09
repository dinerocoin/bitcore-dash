# Bitcore-Dinero

[![NPM Package](https://img.shields.io/npm/v/bitcore-dinero.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-dinero)
[![Build Status](https://img.shields.io/travis/dinerocoin/bitcore-dinero.svg?branch=master&style=flat-square)](https://travis-ci.org/dinerocoin/bitcore-dinero)

Infrastructure to build Dinero and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Dinero Library please see: https://github.com/dinerocoin/bitcore-lib-dinero

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-dinero
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-dinero
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-dinero');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Dinero](https://github.com/dinerocoin/bitcore-node-dinero) - A full node with extended capabilities using Dinero Core
- [Insight API-Dinero](https://github.com/dinerocoin/insight-api-dinero) - A blockchain explorer HTTP API
- [Insight UI-Dinero](https://github.com/dinerocoin/insight-ui-dinero) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/dinerocoin/bitcore-wallet-service-dinero) - A multisig HD service for wallets
- [Wallet Client](https://github.com/dinerocoin/bitcore-wallet-client-dinero) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Dinero wallet

## Libraries

- [Lib-Dinero](https://github.com/dinerocoin/bitcore-lib-dinero) - All of the core Dinero primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Dinero](https://github.com/dinerocoin/bitcore-p2p-dinero) - The peer-to-peer networking protocol
- [Mnemonic-Dinero](https://github.com/dinerocoin/bitcore-mnemonic-dinero) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Dinero transactions
- [Message-Dinero](https://github.com/dinerocoin/bitcore-message-dinero) - Dinero message verification and signing
- [ECIES-Dinero](https://github.com/dinerocoin/bitcore-ecies-dinero) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/dinerocoin/bitcore-dinero/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as DashCore itself. See [LICENSE](LICENSE) for more info.
