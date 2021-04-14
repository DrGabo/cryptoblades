# CryptoBlades

## Getting Started (Crypto)

1. Install [Ganache](https://www.trufflesuite.com/ganache).

1. For Ganache, choose Quickstart Ethereum.

1. Increase the gas limit in the workspace to `67219751`.

1. Install [MetaMask](https://metamask.io/).

1. Create a new connection to connect to Ganache with these settings: http://localhost:7545, any name, any chain id

1. In Ganache, click the key icon on the right side of any address and grab the private key.

1. In MetaMask, create a new account, import from private key, and paste the key in there. 

You should now have 100 fake eth! You're now fake rich.

## Getting Started (Frontend)

1. `npm install`

1. Create a `.env` file in `frontend` with the following values:

- `VUE_APP_CRYPTOBLADES_CONTRACT_ADDRESS`
- `VUE_APP_STAKING_REWARDS_CONTRACT_ADDRESS`
- `VUE_APP_SKILL_TOKEN_CONTRACT_ADDRESS`

## Truffle Environment Variables

Truffle also supports some environment variables, if you create a `.env` file in the root you can specify:

- `ETH_DEV_RPC_HOST`
- `ETH_DEV_RPC_PORT`
- `ETH_DEV_RPC_NETWORK_ID`
- `ETH_DEV_RPC_GAS`
- `BINANCE_WALLET_MNEMONIC`

## Structure

- `contracts` contains the solidity contracts for the game
- `frontend` contains the Vue code for the frontend
- `migrations` contains migration files
- `test` contains tests

## Commands

- `npm run start:frontend` - start up a server for the Vue frontend
- `npm run contract:prepare` - extract the ABI and re-compile Truffle contracts
- `npm run contract:deploy` - deploy the Truffle contracts for testing