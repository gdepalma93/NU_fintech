## Timeseries Analysis

### Curriculum Goal
Gain Proficiency in the following:
    1. Time Series Forecasting
    2. Linear Regression Modeling

### Problem Statement
The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.

In this assignment, we will test a variety of time-series tools to predict future movements in the value of the Japanese yen versus the U.S. dollar.

### File Structure
    1. Time Series Analysis Notebook
    2. Regression Analysis Notebook
    3. Unit Learnings
    4. Yen Historical Data
    
### Time Series Analysis
#### Analysis Process
    1. Decompose using a Hodrick-Prescott Filter (Decompose the Settle price into trend and noise).
    2. Forecast Returns using an ARMA Model.
    3. Forecast the Settle Price using an ARIMA Model.
    4. Forecast Volatility with GARCH.

#### Conclusion
Although the ARIMA model predicts an increase in price in the short term, the ARMA model predicts negative returns and the GARCH model predicts an increase in volatility during same period. Based on the ARMA and Garch Model predictions, I would not buy the yen now.

Based on the upward tend in the GARCH Forecast plot, the exchange risk is expected to increase. 

I hesitate to use HP, ARMA, ARIMA, or GARCH models for trading because they don't take into account outside factors. 



### Linear Regression Analysis
#### Analysis Process
    1. Data Prep (Creating Returns and Lagged Returns and splitting the data into training and testing data)
    2. Fitting a Linear Regression Modelg
    3. Making predictions using the testing data
    4. Out-of-sample performance
    5. In-Sample performance
    
#### Conclusion

Based on the MSE as a measure of prediction error and RMSE as a measure of goodness of fit, out-of-sample performance seems to have less error in predicting returns than in-sample predictions. Based on RMSE the in-sample predictions have a higher goodness of fit.
