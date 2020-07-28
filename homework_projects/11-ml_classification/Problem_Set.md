# Classification Problem Set

## Background
---
Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

In this Problem Set, you will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. 

Files
    - Resources
        - Lending Club Loans Data
    - Starter Files
        - Resampling Notebook
        - Ensemble Notebook
    - Solutions
        - Resampling Solution
        - Ensemble Solution

Libraries
    - Scikit-learn
    - imbalanced learn
    
ML Techniques
    - Resampling
        - Naive Random Oversampling 
        - SMOTE Oversampling
        - Cluster Centroids- Undersampling
        - SMOTEENN - Combination of Over and Under Sampling
    - Ensemble Learning
    
ML Models
    - logistic regression classifier
    - balanced random forest classifier
    - easy ensemble AdaBoost classifier
    
Outputs
    - balanced accuracy score
    - confusion matrix
    - imbalance classification report
    
--- 

## Problem Set
    1. Resampling
        1.1) Resample Data
            1.1.a) Oversample the data using the Naive Random Oversampler and SMOTE algorithms
            1.1.b) Undersample the data using the CLuster Centroids algorithm
            1.1.c) Over-and under-sample using a comination SMOTEENN algorithm
        1.2) Train models for resampled data
            1.2.a) Train a logistic regression classifier from sklearn.linear_model using the resampled data.
            1.2.b) Calculate the balanced accuracy score from sklearn.metrics
            1.2.c) Calculate the confusion matrix from sklearn.metrics
            1.2.d) Print the imbalanced classification report from imblearn.metrics
        1.3) Answer the Following Questions
            1.3.a) Which model had the best balanced accuracy score?
            1.3.b) Which model had the best recall score?
            1.3.c) Which model had the best geometric mean score?
    2. Ensemble Learning
        2.1) Random Forest Classification
            2.1.a) Train the model using the quarterly data from LendingClub provided in the Resource folder.
            2.1.b) Calculate the balanced accuracy score from sklearn.metrics.
            2.1.c) Print the confusion matrix from sklearn.metrics
            2.1.d) Generate a classification report using the imbalancd_classification_report from imbalanced learn
            2.1.e) print the feature importance sorted in descending order (most important feature to least important) along with the feature score.
        2.2) Easy Ensemble AdaBoost Classification
            2.2.a) Train the model using the quarterly data from LendingClub provided in the Resource folder.
            2.2.b) Calculate the balanced accuracy score from sklearn.metrics.
            2.2.c) Print the confusion matrix from sklearn.metrics
            2.2.d) Generate a classification report using the imbalancd_classification_report from imbalanced learn
        2.3) Answer the Following Questions
            2.3.a) Which model had the best balanced accuracy score?
            2.3.b) Which model had the best recall score?
            2.3.c) Which model had the best geometric mean score?
            2.3.d) What are the top three features?

             