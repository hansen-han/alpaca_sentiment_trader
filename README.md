# alpaca_sentiment_trader
This repository contains a Python trading bot, vader_sentiment_trader.py, that uses sentiment analysis to trade stocks via the Alpaca API.

## Overview
The vader_sentiment_trader bot uses the Twitter API to gather sentiment analysis data for a list of specified stocks. It then places trades on those stocks based on their sentiment, using the Alpaca API. The function uses the Vader Sentiment Analysis library, which provides a score for each tweet on a scale from -1 to 1 based on its positive, negative, and neutral sentiment. The vader_sentiment_trader function calculates the average sentiment score for a given stock and uses that score to decide whether to buy, sell, or hold that stock.


## Usage
To use the vader_sentiment_trader.py script, you will need to provide Twitter and Alpaca API authentication credentials. You will also need to specify a list of stocks to trade and a buy threshold. By default, the function uses the S&P 500 ETF (SPY) and a buy threshold of 0.05.


## Notes
The ```vader_sentiment_trader()``` function is set to run continuously during market hours, checking the sentiment of the specified stocks every 30 minutes. However, you can modify the function to change the frequency of sentiment checks or to run the function for a specified period of time.

The function uses the tweepy library to access the Twitter API, and the alpaca_trade_api library to access the Alpaca API. Make sure you have installed these libraries before running the function.

The function is limited by the rate limits of the Twitter API. Make sure you take this into account when specifying the number of tweets to gather for sentiment analysis.

## Disclaimer
The code and information provided in this repository is for educational purposes only and should not be considered as financial advice. The author is not a financial advisor or broker, and assumes no liability for the use or interpretation of the code and information provided. Use of this code for trading purposes is at your own risk. It is important to do your own analysis and research before making any investment decisions.

## License
This code is licensed under the MIT License. See the LICENSE file for details.