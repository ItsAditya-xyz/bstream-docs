# Using Bstream Webhooks

Bstream webhooks allow you set up integrations that subscribe to a certain blockchain event within your code.
When that event occurs, Bstream makes an HTTP request to the URI provided by you.

## What is a webhook?

In simple terms webhooks are automated messages sent from a server when a specific event happens. You can catch a webhook message via a simple API endpoint.
After catching the message, you can execute specific functions as per your needs.

![webhook](https://pbs.twimg.com/media/GAPppGGbUAAGNqZ?format=jpg&name=large)

## Listening to Bstream webhooks

### Creating a webhook

Webhook URI is a simple API endpoint that you can set up to receive webhook messages. You can use replit.com to set up a flask server for testing webhook messages. [Here](https://replit.com/@aditya194/Python#main.py) is a simple flask server that you can use to test webhook messages.

```python
from flask import Flask, request
import json
app = Flask(__name__)

@app.route('/')
def helloWorld():
  return "Simple Flask Server to test Bstream Webhooks"

@app.route('/bstream-webhook', methods=['POST'])
def receive_payload():
  if request.method == 'POST':
    data = request.get_data()
    print("Received Payload:", data)

    '''Now you can execute your function whenever any on-chain event happens. Be it someone
    buying/selling/transferring something etc.'''

    return f"Received webhook data: {data}", 200

  return 'Invalid Request', 400

if __name__ == '__main__':
  app.run(host='0.0.0.0', port=8080)
```

### Adding webhook URI to Bstream

1.  Go to [Bstream](https://Bstrea.io) and click add Stream

    ![add stream](https://media.discordapp.net/attachments/1150445520154808413/1180874316213137419/image.png?ex=657f01e8&is=656c8ce8&hm=f567e8808931a2a272af2f9e5055d1f355ae4c4eb67a87664f2054327596437e&=&format=webp&quality=lossless)

2.  Now select the type of event your want to stream within your code. For instance we will choose 'Transfers' to stream all USDT transactions above $1M

    ![streamType](https://pbs.twimg.com/media/GAPpseFbsAACWnA?format=jpg&name=medium)

3.  Fill the form according to your need. Here we have added token address of USDT which is `0xdac17f958d2ee523a2206206994597c13d831ec7` and set the minimum amount to $1M

    ![stream filters](https://pbs.twimg.com/media/GAPptezasAA7l_d?format=png&name=medium)

4.  Now click add webhook button from integration section

    ![add webhook](https://pbs.twimg.com/media/GAPpuIFacAE9l4p?format=png&name=medium)

5.  Enter the webhook URI, webhook label and any optional headers (if required) and click Finish
    ![webhook](https://pbs.twimg.com/media/GAPpuvOa4AAPCta?format=png&name=900x900)

    **NOTE**: Make sure your webhook URI private to you. Anyone with access to your webhook URI can send you webhook messages.

6.  After saving it, you will start receive webhook messages of all USDT transactions above $1M. The response message is a json object containing all the details of the transaction.


    | Keys                  | Description                                      |
    | ---------------------- | ------------------------------------------------ |
    | streamName             | The name of the stream                           |
    | subjectTwitterUserName | Twitter username of the subject                  |
    | subjectTwitterName     | Twitter name of the subject                      |
    | subjectAddress         | Ethereum address of the subject                  |
    | blockNumber            | Number of the block                              |
    | blockHash              | Hash of the block                                |
    | hash                   | Transaction hash                                 |
    | from                   | Sender's address                                 |
    | to                     | Receiver's address                               |
    | gas                    | Gas used in the transaction                       |
    | gasPrice               | Price of gas                                     |
    | maxFeePerGas           | Maximum fee per gas                               |
    | maxPriorityFeePerGas   | Maximum priority fee per gas                      |
    | nonce                  | Transaction nonce                                |
    | chainId                | Chain ID                                         |
    | transactionIndex       | Index of the transaction in the block             |
    | type                   | Type of transaction                              |
    | value                  | Value sent in the transaction                    |
    | v                      | V parameter of the transaction                   |
    | r                      | R parameter of the transaction                   |
    | s                      | S parameter of the transaction                   |
    | input                  | Input data of the transaction                    |
    | accessList             | List of access information                        |
    | functionName           | Name of the function called in the transaction    |
    | buyer                  | Address of the buyer                             |
    | numberOfSharesToBuy    | Number of shares to buy                           |
    | receiptStatus          | Status of the transaction receipt                 |
    | address                | Address in the log                                |
    | topic0                 | Topic 0 in the log                                |
    | topic1                 | Topic 1 in the log                                |
    | topic2                 | Topic 2 in the log                                |
    | topic3                 | Topic 3 in the log                                |
    | data                   | Data in the log                                   |
    | eventName              | Name of the event logged                          |
    | trader                 | Address of the trader                             |
    | subject                | Address of the subject                            |
    | isBuy                  | Indicates if it's a buy transaction              |
    | shareAmount            | Amount of shares involved in the transaction      |
    | ethAmount              | Amount of Ethereum involved in the transaction    |
    | protocolEthAmount      | Amount of Ethereum for the protocol               |
    | subjectEthAmount       | Amount of Ethereum for the subject                |
    | supply                 | Supply information                                |
