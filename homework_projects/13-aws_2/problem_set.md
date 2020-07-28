# Clustering Crypto Problem Set

## Background
---

You are a Senior Manager at the Advisory Services team on a Big Four firm, and one of your most important clients, a prominent investment bank, is interested in offering a new cryptocurrencies investment portfolio for its customers, however, they are lost in the immense universe of cryptocurrencies, so they ask you to present a report of what cryptocurrencies are on the trading market and how cryptocurrencies could be grouped towards creating a classification for developing this new investment product.

In this homework problem set, you have the opportunity to put in action your new unsupervised learning and Amazon SageMaker skills to cluster cryptocurrencies and create some plots to present your results.


### Files
    - problem_set
    - starter_files
        - crypto_clustering.ipynb
        - Resources
            - crypto_data.csv
    - solution
        - crypto_clustering.ipynb
        - crypto_clustering_sm.ipynb
        - Resources
            - crypto_data.csv
            
### Libraries
    - ML Libraries
        - sklearn
    - visualization libraries
        - hvplot
        - plotly
        
### ML Techniques
    - K-Means Clustering
    - Principal Component Analysis (PCA)
    
### ML Outputs
    - PCA Dataframe
    - elbow curve to find k
    - 3D-Scatter with K-Means Clusters
    - scatter plot to compare total coins mined vs total coin supply
--- 

## Problem Set
    1. Data Preprocessing: Prepare Data for dimension reduction with PCA and clustering using K-Means
        1.1) load data into Pandas Dataframe
        1.2) Remove all cryptos that are not trading
        1.3) Remove all cryptos that do not have an algorithm defined
        1.4) Remove the IsTrading column
        1.5) Remove all cryptos with at least one null value
        1.6) Remove all cryptos without coins mined
        1.7) store the names of all cryptos in a DataFrame named coins_name, use the crypto_df.index as the index for this new dataframe
        1.8) Remove the CoinName column
        1.9) Create dummies variables for all the tesxt features, store the resulting data on a DataFrame named X.
        1.10) Use the StandarScaler from sklearn to standardize all the data of the X DataFrame. Remember this is important prior to using PCA and K-Means Algorithms.
        
    2. Reducing Data Dimensions Using PCA: Reduce data dimension using the PCA algorithm from sklearn
        2.1) Use the PCA algorithm from sklearn to reduce the dimensions of the X DataFrame down to three principal components. 
        2.2) Once you have reduced the data dimensions, create a DataFrame named pcs_df using as columns names "PC 1", "PC 2" and "PC 3";  use the crypto_df.index as the index for this new DataFrame.
        
    3. Clustering Cryptocurrencies Using K-Means: Predict clusters using the cryptocurrencies data using the KMeans algorithm from sklearn.
        3.1) Create an Elbow Curve to find the best value for k, use the pcs_df DataFrame.
        3.2) Once you define the best value for k, run the Kmeans algorithm to predict the k clusters for the cryptocurrencies data. Use the pcs_df to run the KMeans algorithm.
        3.3) Create a new DataFrame named clustered_df, that includes the following columns "Algorithm", "ProofType", "TotalCoinsMined", "TotalCoinSupply", "PC 1", "PC 2", "PC 3", "CoinName", "Class". You should maintain the index of the crypto_df DataFrames as is shown bellow.
    4. Visualizing Results: Create some plots and data tables to present your results.
        4.1) Create a 3D-Scatter using Plotly Express to plot the clusters using the clustered_df DataFrame. You should include the following parameters on the plot: hover_name="CoinName" and hover_data=["Algorithm"] to show this additional info on each data point.
        4.2) Use hvplot.table to create a data table with all the current tradable cryptocurrencies. The table should have the following columns: "CoinName", "Algorithm", "ProofType", "TotalCoinSupply", "TotalCoinsMined", "Class"
        4.3) Create a scatter plot using hvplot.scatter, to present the clustered data about cryptocurrencies having x="TotalCoinsMined" and y="TotalCoinSupply" to contrast the number of available coins versus the total number of mined coins. Use the hover_cols=["CoinName"] parameter to include the cryptocurrency name on each data point.
    5. Deploy your notebook to Amazon SageMaker
        5.1) Upload your Jupyter notebook and rename it as crypto_clustering_sm.ipynb
        5.2) Select the conda_python3 environment.
        5.3) nstall the altair library
        5.4) Use the altair scatter plot to create the Elbow Curve.
        5.5) Use the altair scatter plot, instead of the 3D-Scatter from Plotly Express, to visualize the clusters. Since this is a 2D-Scatter, use x="PC 1" and y="PC 2" for the axes, and add the following columns as tool tips: "CoinName", "Algorithm", "TotalCoinsMined", "TotalCoinSupply".
        5.6) Use the altair scatter plot to visualize the tradable cryptocurrencies using  x="TotalCoinsMined" and y="TotalCoinSupply" for the axes.
        5.7) Show the table of current tradable cryptocurrencies using the display() command.
        5.8) Remove all hvplot and Plotly Express references from your code.