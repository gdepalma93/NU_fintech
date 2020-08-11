# NU Fintech Project 2
--- 

## ML Problem Formulation

    1. Articulate your problem
        - maximize risk adjusted algorithmic trading returns using skills learned in NU Fintech class
        - simulate a quant trading desk
        - machine learning- multi-factor classification model (gradient boosters, random forests, logistic regression)
    2. Start Simple
        - factor research notebook 
            - universe selection
                - cryptocurrencies
                    - kraken
                    - bittrex
                    - coinbase
            - signal generation
                - sentiment calculus- (ibm-tone analyzer, nltk-intensity analyzer), event 
                - momentum cross sectional- (long only)- nueral net
                - technical- ema cross, volatility, RSI
                - fundamental- factor-based investing (crypto clustering homework)- principal component analysis
        - algorithmic trading framework
            - initialize
            - build dashboard
            - fetch data
            - generate signals
            - execute_trade_strategy
            - evaluate metrics
            - execute backtest
            - main
        - train system with ML Model to optimize for risk adjusted returns (regularization modeling) --areas to improve
        - implement trading framework on AWS (Sagemaker) // deploy on spyder or visual studio or pycharm
        - automate performance reporting ()
    3. Identify Data Sources
        - Shrimpy- crypto price data
        - newsapi- sentiment signal
        - twitter- sentiment signal
        - crypto compare - fundamental signal
    4. Design Data For Model
        - multi-level dataframe
    5. Determine where data comes from
        - shrimpy, newsapi, twitter
    6. Determine easily designed inputs
        - shrimpy, newsapi, twitter
    7. ability to learn
        - random forest, gradient boosters, logistic regression
    8. Potential bias
        - 
    
## NU Fintech Notebooks
    - cryptoclustering
    - ibm tone analyzer
    - nltk instensity analyzer
    - random forest trading (Signal, training, trading)
    - logistic regression notebooks
    - gradient booster notebooks
    - k-means clustering notebooks
    - lstm-tensorflow-keras notebooks


## Links
[problem formulation](https://developers.google.com/machine-learning/problem-framing/formulate)  
[alphalens](https://www.quantopian.com/docs/api-reference/alphalens-api-reference#alphalens.utils.get_clean_factor_and_forward_returns) 
[shrimpy github](https://github.com/shrimpy-dev/shrimpy-python)  
[shrimpy developer](https://developers.shrimpy.io/docs/?python#rebalancing)  
[nu fintech project 1](https://github.com/gdepalma93/quantitative_trading_system)
[Crypto CLustering Homework](https://nu.bootcampcontent.com/NU-Coding-Bootcamp/nu-chi-fin-pt-04-2020-u-c/tree/master/02-Homework/13-AWS-Lex/Instructions)  
[cryptocompare](https://www.cryptocompare.com/)  
[news api](https://newsapi.org/docs/endpoints/sources)  
[developer twitter](https://developer.twitter.com/en/docs/basics/authentication/api-reference/access_token)  
[shrimpy](https://www.shrimpy.io/)  
[shrimpy x coinbase](https://blog.shrimpy.io/blog/python-scripts-for-coinbase-pro-market-data)  
[shrimpy trading bot](https://blog.shrimpy.io/blog/how-to-make-a-crypto-trading-bot-using-python)  
[shrimpy api](https://blog.shrimpy.io/blog/how-to-make-a-crypto-trading-bot-using-python)  

[nltk](https://www.nltk.org/api/nltk.sentiment.html)  
[ibm watson](https://www.ibm.com/watson/services/tone-analyzer/)  
[python pandas multiindexing](https://pandas.pydata.org/pandas-docs/stable/user_guide/advanced.html)  
[iterate over rows in pandas](https://stackoverflow.com/questions/16476924/how-to-iterate-over-rows-in-a-dataframe-in-pandas)  
[l1 and l2 regularization methods](https://towardsdatascience.com/l1-and-l2-regularization-methods-ce25e7fc831c)  
[blueshift](https://blueshift.quantinsti.com/research/strategies/3a32abeec97fa9cd5b7ee4f038d208d8/edit) 
[kraken](https://www.kraken.com/)  
[bittrex](https://bittrex.com)  
[coinbase pro](https://pro.coinbase.com/)  
[sagemaker](https://aws.amazon.com/sagemaker/)
[AWS S3 Bucket](https://aws.amazon.com/s3/)  
[AWS Lambda](https://aws.amazon.com/lambda/)  

[cryptocompare pypi](https://pypi.org/project/cryptocompare/)  






