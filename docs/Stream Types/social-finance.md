# SocialFi

Using **Social Fi** stream on can receive notifcations related to SoFi platforms like FriendTech.

## Supported Platforms:

- **FriendTech**

The SocialFi stream has below filters:

![stream filters](https://cdn.discordapp.com/attachments/841605440038240276/1181916576883146853/image.png?ex=6582cc96&is=65705796&hm=d7e0e0c00eaa62ad7a68ef3c233b3f0fb75e89b62cf63c49aaabeea35ac92e89&)

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

## Message Parameters

    ![params](https://cdn.discordapp.com/attachments/841605440038240276/1181922176190918686/image.png?ex=6582d1cd&is=65705ccd&hm=8ad7d4d300466090e0ffceb8eccd3e5915004d769829fad47794265d53178415&)

| Message Parameters    | Description                                  |
| --------------------- | -------------------------------------------- |
| Stream Name           | Returns Stream Name                          |
| Twitter Handle        | Twitter Handle of trader                     |
| Account Address       | Account address of trader                    |
| Date & Time Addresses | Returns the date and time of the transaction |
| Txn link              | Returns the scan link of the transfer        |
| Follower Count        | Follower count on twitter                    |
| Twitter Profile       | Twitter address of subject key               |
