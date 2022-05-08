# Credit_Risk_Analysis

## Overview
The overview of this analysis is to use Python to build and evaluate several machine learning models to predict credit risk. 

## Purpose
Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud.

## Results
  - Oversampling - RandomOverSampler algorithm
     - Acuuracy score - 0.5439153831192286
     - Confusion matrix - array([[   70,    31],[10352,  6752]], dtype=int64)
     - Classification report
    ![2](https://user-images.githubusercontent.com/95719819/166175652-06ee1e8b-5060-4a1b-890a-b91f61016b7b.png)

  - Oversampling - SMOTE algorithm
     - Acuuracy score - 0.6622479600626106
     - Confusion matrix - array([[   64,    37],[ 5288, 11816]], dtype=int64)
     - Classification report
     
    ![1](https://user-images.githubusercontent.com/95719819/166175629-5e5c2d57-6f0b-4680-82ae-fee54f286aea.png)

  - Undersampling - ClusterCentroids algorithm
     - Acuuracy score - 0.5442661782548694
     - Confusion matrix - array([[   70,    31],[10340,  6764]], dtype=int64)
     - Classification report
    ![3](https://user-images.githubusercontent.com/95719819/166175691-51c6aa63-7f19-43c9-a2c9-0a725e8c8828.png)

  - Combinatorial(Over-and undersampling) - SMOTEENN algorithm
     - Acuuracy score - 0.644711676499736
     - Confusion matrix - array([[  73,   28],[7412, 9692]], dtype=int64)
     - Classification report
     
    ![4](https://user-images.githubusercontent.com/95719819/166175709-9cd7df9a-4b05-418e-a888-c879602d1c0a.png)

  - Ensemble classifiers - BalancedRandomForestClassifier algorithm
     - Acuuracy score - 0.7833251991561447
     - Confusion matrix - array([[   70,    34],[ 1820, 15281]], dtype=int64)
     - Classification report
    ![5](https://user-images.githubusercontent.com/95719819/166175724-6f238b8c-b53f-4ff3-8d4e-a6ba6d2e630e.png)

  - Ensemble classifier - EasyEnsembleClassifier algorithm
     - Acuuracy score - 0.9178773283613644
     - Confusion matrix - array([[   93,    11],[ 1000, 16101]], dtype=int64)
     - Classification report
  ![6](https://user-images.githubusercontent.com/95719819/166175738-69c16aec-3243-4ea7-b33e-e6c9bc1fdd5c.png)

## Summary
  - The Summary of our analysis is that, in all the algorithms first we created training and target variables and the balance of the target variables are checked. Then resampling is done on training variables with the respective algorithms to calculate the accuracy score, generate a confusion matrix and print out the imbalanced classification report.

  - I recommend EasyEnsembleClassifier model for credit risk analysis because, our results show that the EasyEnsembleClassifier has the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
