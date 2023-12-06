# Transfers

Using **Transfers** stream on can receive notifcations about transfer of tokens on chains like Ethereum, Arbitrum etc.

Supported Networks:

Ethereum mainnet
Arbitrum

![stream filters](https://cdn.discordapp.com/attachments/841605440038240276/1181900554759307294/image.png?ex=6582bdaa&is=657048aa&hm=6686a4d09f53219d93cd500b974d6a45b39d10e34c9e62c403bf7fcaa6e5406f&)

## Filter Parameters

| Chain            | Chain to monitor on                             |
| ---------------- | ----------------------------------------------- |
| Operator         | Filter on transfer amounts                      |
| Amount           | Filter on amounts                               |
| Currency         | Automatically chosen upon selecting the network |
| Wallet Addresses | Monitor up to 5 wallets                         |

## Message Params

    ![params](https://docs.bstream.io/assets/images/native-transactions-message-f1b6ba4547a85d28417fe0e273e60e63.png)

| Stream Name           | Returns the name of the stream               |
| --------------------- | -------------------------------------------- |
| Token                 | Returns the token trasnacted                 |
| From                  | Returns the sender's wallet                  |
| To                    | Returns the receiver's wallet                |
| Chain                 | Returns the chain                            |
| Date & Time Addresses | Returns the date and time of the transaction |
| Txn link              | Returns the scan link of the transfer        |
