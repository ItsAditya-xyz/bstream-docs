# Smart Contracts

Using **Smart Contracts** alerts, one receive notifications of smart contract functions and events.

## Supported Networks:

1. **Ethereum mainnet**
2. **Arbitrum**

![stream filters](https://cdn.discordapp.com/attachments/841605440038240276/1185140314667765781/image.png?ex=658e86ed&is=657c11ed&hm=d20b8af73ee4933afc1c283d5923322ff5a05041811b6fa7ee685e53a03209df&)

## Filter Parameters

| Filter Type      | Description                                                                                                               |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Chain            | Chain to track, eg. Ethreum, avax, arbitrum etc.                                                                          |
| Contract Address | Address of the contract you want to track                                                                                 |
| Contract ABI     | Automatically fetched after contract address is added. It is a json data that defines contract function and its structure |
| Monitor By       | Can be **function** or **event**                                                                                          |
| Parameters       | Custom Parameters (optional)                                                                                              |

## Message Parameters

    ![params](https://cdn.discordapp.com/attachments/841605440038240276/1185143571779686400/image.png?ex=658e89f6&is=657c14f6&hm=7b6798ffb3e5e03f9056568e77d88319ba0ba94400f36681888dda09527abcf3&)

| Message Parameter | Description                                  |
| ----------------- | -------------------------------------------- |
| Stream Name       | Returns the name of the stream               |
| Contract Name     | Name of the contract                         |
| Event/Function    | Event or Function that was called.           |
| Parameters        | Extra data of the transaction                |
| Chain             | Returns the chain                            |
| Date & Time       | Returns the date and time of the transaction |
| Txn link          | Returns the link of the transfer             |
