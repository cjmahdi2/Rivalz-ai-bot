# Rivalz AI Bot

This repository contains a bot for interacting with the Rivalz Fragmentz claimer using Ethereum wallets.

## Features

- Check wallet balances
- Claim Fragmentz
  - One-time claim
  - Recurring claim every 12 hours
- Interactive CLI interface

## Getting Started

Follow these steps to set up and run the bot.

Log in to the site And Get faucet for them here:
https://rivalz2.hub.caldera.xyz/

### Install Node.js And npm:
```
sudo apt update && apt upgrade -y
sudo apt remove nodejs
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash
source ~/.bashrc
nvm install 22.9.0
nvm use 22.9.0
nvm alias default 22.9.0
```
### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/cjmahdi2/Rivalz-ai-bot.git
   cd Rivalz-ai-bot
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

### Setting Up Wallets

You need to provide your Ethereum private keys or mnemonics in either ```nano privateKeys.json``` or ```nano accounts.json``` in the following formats:

- For private keys (array of strings):

  ```json
  [
    "private_key_1",
    "private_key_2"
  ]
  ```

- For mnemonics (array of strings):

  ```json
  [
    "banana apple boat monkey",
    "chicken dog cat ball"
  ]
  ```

### Usage
Creating a Screen:
```
screen -S Rivalz-ai-bot
```

To start the bot, run:

```bash
npm start
```

#### Options

1. **Check Balances**: Enter `0` to check the balance of each wallet.
2. **Claim Fragmentz**: Enter `1` to claim Fragmentz.
   - **One-time Claim**: Enter `1` to claim once.
   - **Recurring Claim**: Enter `2` to perform an initial claim and set up a recurring job that runs every 12 hours.

## Donations

If you would like to support the development of this project, you can make a donation using the following addresses:

- **Solana**: `DhvXt1hSvkhMwyVvPVwTF5ge1qgKT1sHgnknS4wtnLsG`
- **EVM**: `0x83F129E662B21cF035bc9510f65eb29C75b69155`

## License

This project is licensed under the [MIT License](LICENSE).
