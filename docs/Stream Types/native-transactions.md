# Native Transaction

Using **Native Transactions** one receive notifications about transfers of native currencies like Ethereum, Avax etc.

## Supported Networks:

1. **Ethereum mainnet**
2. **Arbitrum**

![stream filters](https://cdn.discordapp.com/attachments/841605440038240276/1181907422604951652/image.png?ex=6582c410&is=65704f10&hm=5de87bebb2b7250aa0e0f3fd095969f2639b54fd73efc884fe13534c790234fd&)

## Filter Parameters

| Filter Type        | Description                                                       |
| ------------------ | ----------------------------------------------------------------- |
| Chain              | Chain to track, eg. Ethreum, avax, arbitrum etc. |
| Wallet Address     | List of wallets you want to track (optional).                     |
| Operators          | Less then, more than or equal to a specific amount                  |

## Message Params

    ![params](https://docs.bstream.io/assets/images/native-transactions-message-f1b6ba4547a85d28417fe0e273e60e63.png)

| Stream Name           | Returns the name of the stream               |
| --------------------- | -------------------------------------------- |
| Token                 | Returns the token trasnacted                 |
| From                  | Returns the sender's wallet                  |
| To                    | Returns the receiver's wallet                |
| Chain                 | Returns the chain                            |
| Date & Time Addresses | Returns the date and time of the transaction |
| Txn link              | Returns the link of the transfer        |
