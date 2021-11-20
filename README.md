# BSCTokenTracker
A Program to track all transactions on the blockchain for tokens sent to your wallet address. The tokens are then tracked until a Take Profit point where they are then sold.

Setup:
- pip install -r requirements.txt
- Add your Wallet address to config.txt
- Add your Private Key to config.txt

How it Works:
- The program tracks all transactions going through the blockchain and only searches for ones coming from your wallet. It gets the contract address of the token you bought and starts a new thread to track the price. It currently has a stop loss at 20% and a trailing take profit at 5%. This can be changed easily though.

Issues:
- Sell function currently doesn't work
