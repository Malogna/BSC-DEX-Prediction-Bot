# DEXPredictionBot (Malogna version)

This bot fetches the overall consensus of the 5min and 1min BNB/USDT charts based on a number of TA signals provided by Trading View. It determines if the consensus is a BUY or SELL prior to each prediction round and places the bet on PancakeSwap or CandleGenie accordingly.

## What is this fork?
The original code for this created by jontstaz had an automatic "donation" function before every tx. It never worked as intended and most of the times just took half of your BNB. This fork:
- Removes the donation function
- Makes the wait for the bet closer to the close, creating a more accurate bet. (Change this in /src/index.ts if you experience failed TXs)


## NFA and DYOR!

## 💡 How to use

1. Install [Node.JS](https://nodejs.org/en/download/)
2. Clone this repository
3. Extract
4. Edit `.env-example` with your private key and desired bet amount, then rename to `.env`
5. run `npm install` in a command prompt in the folder
6. For PancakeSwap run `npm run start`. For CandleGenie run `npm run candle` (I don't know if CandleGenie works.)
7. ???
8. Profit



#### Advice:
- Set your bet amount to no higher than 1/10th of your available BNB balance.
- Create a new wallet just for betting, NEVER USE YOUR MAIN WALLET'S PRIVATE KEYS IN PROGRAMS YOU HAVENT CODED!


## Disclaimers

There is no sure win rate to this program, because... bsc markets. Right now its around 45%-70%. May change drastically depending on the market. Again, NFA.

**Nothing contained in this program, scripts, code or repository should be construed as investment advice.**

All investment strategies and investments involve risk of loss.
By using this program you accept all liabilities, and that no claims can be made against the developers or others connected with the program.
Credits to Modagavr for original build. I extended the bot greatly to make it much smarter as opposed to just following/going against the trend of other bettors.
