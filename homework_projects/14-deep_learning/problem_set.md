# Deep Learning Problem Set

## Background
---

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the Crypto Fear and Greed Index (FNG) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. You have been asked to help build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

In this Problem Set, you will use deep learning recurrent neural networks to model bitcoin closing prices. One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

### Files
    - README.md (problem set description)
    - starter_files
        - btc_historic.csv
        - btc_sentiment.csv
        - lstm_stock_predictor_closing.ipynb
        - lstm_stoc_predictor_fng.ipynb
    - solutions
        - btc_historic.csv
        - btc_sentiment.csv
        - lstm_stock_predictor_closing.ipynb
        - lstm_stoc_predictor_fng.ipynb
        
### Libraries
    - ML Libraries
        - tensorflow
        - Keras
    - data science libraries
    
    
### Deep Learning Techniques
    - Keras Sequential Model
    - Keras LSTM, Dense, Droput layers
### Deep Learning Models
    - LSTM Recurrent Neural Networks
    
---

## Problem Set
    1. Prepare the data for training and testing
    2. Build and train custom LSTM Recurrent Neural Networks
    3. Evaluate the Performance of Each Model
        3.1) Which model has a lower loss?
        3.2) Which model tracks the actual values better over time?
        3.3) Which windo size works best for the model?