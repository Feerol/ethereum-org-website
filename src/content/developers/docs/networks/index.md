---
title: Networks
description: An overview of Ethereum's networks and where to get testnet ether (ETH) for testing your application.
lang: en
sidebar: true
preMergeBanner: true
---

Networks are different Ethereum environments you can access for development, testing, or production use cases. Since Ethereum is a protocol, there can be multiple independent "networks" that conform to the protocol without interacting with each other.

Your Ethereum account will work across the different networks, but your account balance and transaction history won't carry over from the main Ethereum network. For testing purposes, it's useful to know which networks are available and how to get testnet ETH to play around with.

## Prerequisites {#prerequisites}

You should understand the [basics of Ethereum](/developers/docs/intro-to-ethereum/) before reading up on the different networks, as the test networks will give you a cheap, safe version of Ethereum to play around with.

## Public networks {#public-networks}

Public networks are accessible to anyone in the world with an internet connection. Anyone can read or create transactions on a public blockchain and validate the transactions being executed. The consensus among peers decides on the inclusion of transactions and the state of the network.

### Ethereum Mainnet {#ethereum-mainnet}

Mainnet is the primary public Ethereum production blockchain, where actual-value transactions occur on the distributed ledger.

When people and exchanges discuss ETH prices, they're talking about Mainnet ETH.

### Ethereum Testnets {#ethereum-testnets}

In addition to Mainnet, there are public testnets. These are networks used by protocol developers or smart contract developers to test both protocol upgrades as well as potential smart contracts in a production-like environment before deployment to Mainnet. Think of this as an analog to production versus staging servers.

You should test any contract code you write on a testnet before deploying to Mainnet. Among dapps that integrate with existing smart contracts, most projects have copies deployed to testnets.

Most testnets use a proof-of-authority consensus mechanism. This means a small number of nodes are chosen to validate transactions and create new blocks – staking their identity in the process. Testnets do not incentivize proof-of-work mining, which can leave them vulnerable.

ETH on testnets has no real value; therefore, there are no markets for testnet ETH. Since you need ETH to actually interact with Ethereum, most people get testnet ETH from faucets. Most faucets are webapps where you can input an address which you request ETH to be sent to.

#### Sepolia {#sepolia}

A proof-of-work testnet. The best like-for-like representation of Ethereum Mainnet.

- [Website](https://sepolia.dev/)
- [Github](https://github.com/goerli/sepolia)
- [Otterscan](https://sepolia.otterscan.io/)
- [Etherscan](https://sepolia.etherscan.io)

##### Sepolia faucets

- [Sepolia faucet](https://faucet.sepolia.dev/)
- [FaucETH](https://fauceth.komputing.org)

#### Görli {#goerli}

A proof-of-authority testnet that works across clients; an ideal testnet for application developers.

- [Website](https://goerli.net/)
- [Github](https://github.com/goerli/testnet)
- [Etherscan](https://goerli.etherscan.io)

##### Görli faucets

- [Görli faucet](https://faucet.goerli.mudit.blog/)
- [Chainlink faucet](https://faucets.chain.link/)
- [Alchemy Goerli Faucet](https://goerlifaucet.com/)

#### Ropsten _(deprecated)_ {#ropsten}

_Note, [the Ropsten testnet is deprecated](https://github.com/ethereum/pm/issues/460) and will no longer receive protocol upgrades. Please consider migrating your applications to Sepolia or Görli._

A proof-of-work testnet. It only serves historical relevance and is mainly used by core developers for testing protocol upgrades.

##### Ropsten faucets

- [FaucETH](https://fauceth.komputing.org) (multi-Chain faucet without the need for social account)
- [Paradigm faucet](https://faucet.paradigm.xyz/)

#### Rinkeby _(deprecated)_ {#rinkeby}

_Note: [the Rinkeby testnet is deprecated](https://github.com/ethereum/pm/issues/460) and will no longer receive protocol upgrades. Please consider migrating your applications to Sepolia or Görli._

A proof-of-authority testnet for those running old versions of the Geth client.

##### Rinkeby faucets

- [FaucETH](https://fauceth.komputing.org) (multi-Chain faucet without the need for social account)
- [Alchemy faucet](https://RinkebyFaucet.com)
- [Chainlink faucet](https://faucets.chain.link/)
- [Paradigm faucet](https://faucet.paradigm.xyz/)
- [Rinkeby faucet](https://faucet.rinkeby.io/)

#### Kovan _(deprecated)_ {#kovan}

_Note: [the Kovan testnet is deprecated](https://github.com/ethereum/pm/issues/460) and will no longer receive protocol upgrades. Please consider migrating your applications to Sepolia or Görli._

A very old proof-of-authority testnet for those still running OpenEthereum clients.

##### Kovan faucets

- [FaucETH](https://fauceth.komputing.org) (multi-Chain faucet without the need for social account)
- [Chainlink faucet](https://faucets.chain.link/)
- [Paradigm faucet](https://faucet.paradigm.xyz/)

### Layer 2 testnets {#layer-2-testnets}

[Layer 2 (L2)](/layer-2/) is a collective term to describe a specific set of Ethereum scaling solutions. A layer 2 is a separate blockchain that extends Ethereum and inherits the security guarantees of Ethereum. Layer 2 testnets are usually tightly coupled to public Ethereum testnets.

#### Arbitrum Rinkeby {#arbitrum-rinkeby}

A testnet for [Arbitrum](https://arbitrum.io/).

Arbitrum Rinkeby faucets:

- [FaucETH](https://fauceth.komputing.org) (multi-Chain faucet without the need for social account)
- [Chainlink faucet](https://faucets.chain.link/)
- [Paradigm faucet](https://faucet.paradigm.xyz/)

#### Optimistic Kovan {#optimistic-kovan}

A testnet for [Optimism](https://www.optimism.io/).

Optimistic Kovan faucets:

- [FaucETH](https://fauceth.komputing.org) (multi-Chain faucet without the need for social account)
- [Paradigm faucet](https://faucet.paradigm.xyz/)

## Private networks {#private-networks}

An Ethereum network is a private network if its nodes are not connected to a public network (i.e. Mainnet or a testnet). In this context, private only means reserved or isolated, rather than protected or secure.

### Development networks {#development-networks}

To develop an Ethereum application, you'll want to run it on a private network to see how it works before deploying it. Similar to how you create a local server on your computer for web development, you can create a local blockchain instance to test your dapp. This allows for much faster iteration than a public testnet.

There are projects and tools dedicated to assist with this. Learn more about [development networks](/developers/docs/development-networks/).

### Consortium networks {#consortium-networks}

The consensus process is controlled by a pre-defined set of nodes that are trusted. For example, a private network of known academic institutions that each govern a single node, and blocks are validated by a threshold of signatories within the network.

If a public Ethereum network is like the public internet, a consortium network is like a private intranet.

## Related tools {#related-tools}

- [Chainlist](https://chainlist.org/) _list of EVM networks to connect wallets and providers to the appropriate Chain ID and Network ID_
- [EVM-based Chains](https://github.com/ethereum-lists/chains) _GitHub repo of chain metadata that powers Chainlist_

## Further reading {#further-reading}

_Know of a community resource that helped you? Edit this page and add it!_
