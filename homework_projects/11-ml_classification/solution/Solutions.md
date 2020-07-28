## Solutions
---

1. Resampling
    1.1) See credit_risk_resampling notebook
    1.2) See credit_risk_resampling notebook
    1.3) Analysis
        1.3.a) In conclusion, the SMOTEEN Resampling method produced the highest balanced accuracy score (0.6421). 
            - Balanced Accuracy Scores
                - Naive Random Oversampling = 0.6384
                - SMOTE = 0.6421
                - Cluster Centroids = 0.524
                - SMOTEENN = 0.6423            
        1.3.b) In conclusion, the SMOTEEN Resampling method produced the highest recall score (0.7). 
            - Recall Scores
                - Naive Random Oversampling = 0.66
                - SMOTE = 0.61
                - Cluster Centroids = 0.65
                - SMOTEENN = 0.7              
        1.3.c) In conclusion, the Naive Random Oversampler, SMOTE, and SMOTEEN resampling methods all produced the same geometric mean scores (0.64).
            - Geometric Mean Scores
                - Naive Random Oversampling = 0.64
                - SMOTE = 0.64
                - Cluster Centroids = 0.51
                - SMOTEENN = 0.64    
                
2. Ensemble Learning
    2.1) see credit_risk_ensemble notebook
    2.2) see credit_risk_ensemble notebook
    2.3) Analysis
        2.3.a) In conclusion, the balanced AdaBoost Classifer produced the highest balanced accuracy score (0.932)
            - Balanced Accuracy Scores
                - Balanced Random Forest Classifier = 0.785
                - Easy Ensemble AdaBoost Classifier = 0.932
        2.3.b) In conclusion the AdaBoost Classifer produced the highest recall score(0.94)
            - Recall Scores
                - Balanced Random Forest Classifier = 0.67
                - Easy Ensemble AdaBoost Classifier = 0.94
        2.3.c) In conclusion, the AdaBoost Classifer model produced the highest geometric mean score (0.93). 
            - Geometric Mean Scores  
                - Balanced Random Forest Classifier = 0.78
                - Easy Ensemble AdaBoost Classifier = 0.93
        2.3.d) The random Forest Classifier indicates that the top 3 features of Loan prediction are...
            1. Loan Amount: (0.0917)
            2. Interest Rate: (0.0641)
            3. Installment: (0.0573)
            
            
            