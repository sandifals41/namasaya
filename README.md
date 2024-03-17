# HOT miner

A script to automatically mine HOT every 2 hours.

## Setup

- Install Nodejs here https://nodejs.org/en, recommended download LTS version 20.11.0
- Clone repository `git clone https://github.com/asepkh/hot-miner-auto-claim.git`, login git first if needed, or you can download via zip.
- run `cd ./hot-miner-auto-claim`
- Install yarn via `npm i -g yarn`
- Install pm2 via `npm i -g pm2`
- Install dependencies via running `yarn`
- Paste your multiple account ID and private key without the `ed25519:` prefix, to be execute hot miner auto claim in `wallets.json`

```sh
# example
[
  {
    "publicKey": "HOT_WALLET_PUBLIC_KEY_1, example: asepkh.near",
    "privateKey": "PRIVATE_KEY_1"
  },
  {
    "publicKey": "HOT_WALLET_PUBLIC_KEY_2, example: asepkh.near",
    "privateKey": "PRIVATE_KEY_2"
  },
  {
    "publicKey": "ANOTHER_MULTIPLE_FOLLOW_THIS_PATTERN",
    "privateKey": "..."
  }
]
```

## Run

Run via pm2:

```sh
# run script
pm2 start hot-miner.config.js
```
