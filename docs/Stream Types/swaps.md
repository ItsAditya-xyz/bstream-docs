# Swaps

Using **Swaps** stream on can receive notifcations about swapping of tokens that happens on decentralzied exchanges like Uniswap.

## Supported Networks:

- **Ethereum mainnet**
- **Arbitrum**

## Supported Protocol (DEX):

- **Uniswwap-V2**
- **Uniswap-V3**

The Swaps stream has below filters:

![stream filters](https://media.discordapp.net/attachments/841605440038240276/1181911119284154388/image.png?ex=6582c781&is=65705281&hm=100064d8d057a94d6bf36c8ee7077e84942c109fde927f906d88b411fcc7e397&=&format=webp&quality=lossless&width=684&height=687)

## Filter Parameters

| Filter Type    | Description                                        |
| -------------- | -------------------------------------------------- |
| Chain          | Chain on which the swaps are executed              |
| Protocol       | DEX Protocol on which the swaps are executed       |
| Wallet Address | List of wallets you want to track (optional).      |
| Token          | Token address for one pair                         |
| Operators      | Less then, more than or equal to a specific amount |
| Swap Direction | Whether the swap is buy, sell or both              |
| Pair           | Select pairs you want to track.                    |

:::note Note
If no pair is specified, all pairs in the network will be included
:::

## Message Params

    ![params](https://docs.bstream.io/assets/images/swap-message-832d160866664773ff3a800a941bd2f9.png)

| Message name | Description                                  |
| ------------ | -------------------------------------------- |
| Stream Name  | The name of the stream                       |
| Wallet       | wallet address of the trader                 |
| Token Out    | Returns the sold token                       |
| Token In     | Returns the bought token                     |
| Protocol     | Returns the swap protocol                    |
| Swap Price   | Returns the price of bought token            |
| Date & Time  | Returns the date and time of the transaction |
| Txn link     | Returns the link of the transaction          |
