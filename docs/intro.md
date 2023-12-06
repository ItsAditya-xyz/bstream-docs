---
sidebar_position: 1
---

# BStream Overview

## What is Bstream?

Bstream is a blockchain data streaming platform that allows users to create custom streams and receive real-time notifications about on-chain events within apps like telegram, discord, email, or through webhooks.

## Why Bstream?

1. Stay informed about on-chain events in real-time - monitor wallets, tokens and contracts to stay in touch with on-chain information you need.
2. No-code solution to receive alerts
3. Works within your favorite apps like telegram or discord
4. Build custom tools with real time data using webhooks integration.
5. Supports renowed blockchains like Ethereum, Arbitrum, Base etc. More coming soon.

## How does Bstream works?

Bstream extracts every new registered block on the ledger and loads it through our workflows. The data runs through defined filters by the users and executes the integration method for each filter. All of it is done within less then a second to assure the alerts reach to the users in fastest possible way.

## Practical use-cases:

- **Copy traders**: Users can follow trader's wallets activities. Whether it is a swap, transfers or other derivative trades. They will be the first to get notified when the trader interacts with the network and act accordingly
- **Avoid getting rugged**: Users can follow the project owner's treasury wallet and monitor the activity of the token they invested in. They will be the first to know when owners list their NFTs, receive a big amount of the token from the smart contract, or if they start selling the project's tokens. Our instant notifications system helps prevent traders loosing money in DeFi.
- **Build tools using real time on-chain data**: Using Bstream's webhook integration, one can receive real time data within code. Using weebhooks, one can build tools like 'rug proof' trading bots, analytics platform and more! Imaginations got no ceilings.

## Getting Started

1. Create an account on [Bstream.io](https://bstream.io) using your email. No wallet login required.

2. In the app's dashboard section, go to Streams section (on the left side of the menu)

   ![image](https://docs.bstream.io/assets/images/stream-sidebar-a1b529a213cbaecb4c79f043f2f8fd9e.png)

3. Click on Add Stream button

   ![add stream](https://cdn.discordapp.com/attachments/1150445520154808413/1180874316213137419/image.png?ex=657f01e8&is=656c8ce8&hm=f567e8808931a2a272af2f9e5055d1f355ae4c4eb67a87664f2054327596437e&)

4. Pick your Stream type

   ![streamType](https://docs.bstream.io/assets/images/transaction-types-ac802b65c25028b55a539438fd431e46.png)

Bstream provides a wide range of Stream types:

- **Native Transactions**: For tracking native coins like Ethereum.
- **Transfers**: For tracking tokens.
- **Swaps**: To track swaps executed on Decentralized exchanges
- **Socialfi**: To track Social Finance tokens and native keys like that of FriendTech.
- **Smart Contracts** (coming soon): To track custom smart contract events.
- **Liquidity Pools** (coming soon):
- **Perpetual Trades** (coming soon)
- **Options Trades** (coming soon)

5. After selecting Stream types, you fill custom filters according to your needs. Different stream types require different types of filters. For example, if you have selected **Transfers**, you have to fill chain name, wallet address (optional) and token address (the token you want to track the transfers of)

   ![image](https://docs.bstream.io/assets/images/stream-filters-c88665fe13636daabe5c7c3833b8313a.png)

6. Select your platform where you want to receive the notifications. Currently we provide alerts via telegram and webhook.

   ![image](https://pbs.twimg.com/media/GAPpuIFacAE9l4p?format=png&name=small)

    Supported Integrations:
    - **Telegram**: You will have to create a telegram bot yourself by following these steps:
        ![image](https://cdn.discordapp.com/attachments/1168052694901075978/1181898047345655889/image.png?ex=6582bb55&is=65704655&hm=88abc60887770a397bf8b418e8aff3dd92d1c73ccfd4cde9320bf4263c6e6acd)
    - **Webhook**: To receive alerts within your webhook servers, simply add your webhook URI:
        ![image](https://pbs.twimg.com/media/GAPpuvOa4AAPCta?format=png&name=900x900)
    - **Discord** (coming soon)
    - **Email** (coming soon)
