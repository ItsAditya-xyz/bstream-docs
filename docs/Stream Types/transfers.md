# Transfers

Using **Transfers** stream on can receive notifcations about transfer of tokens on chains like Ethereum, Arbitrum etc.

## Supported Networks:

- **Ethereum mainnet**
- **Arbitrum**

The transfers stream has below filters:
![stream filters](https://cdn.discordapp.com/attachments/841605440038240276/1181900554759307294/image.png?ex=6582bdaa&is=657048aa&hm=6686a4d09f53219d93cd500b974d6a45b39d10e34c9e62c403bf7fcaa6e5406f&)

## Filter Parameters

| Filter Type        | Description                                                       |
| ------------------ | ----------------------------------------------------------------- |
| Chain              | Chain on which the token is deployed. eg. Ethereum, Arbitrum etc. |
| Wallet Address     | List of wallets you want to track (optional).                     |
| Transfer direction | In, out or both.                                                  |
| Token address    | Token address you want to track.                                  |
| Operators          | Less then, more than or equal to a specific amount                  |

:::note Note
If no wallet is provided, all transfers of the token will be streamed
:::

## Message Params

    ![params](https://docs.bstream.io/assets/images/native-transactions-message-f1b6ba4547a85d28417fe0e273e60e63.png)

| Stream Name           | Returns the name of the stream               |
| --------------------- | -------------------------------------------- |
| Token                 | Returns the token transacted                 |
| From                  | Returns the sender's wallet                  |
| To                    | Returns the receiver's wallet                |
| Chain                 | Returns the chain                            |
| Date & Time Addresses | Returns the date and time of the transaction |
| Txn link              | Returns the scan link of the transfer        |
