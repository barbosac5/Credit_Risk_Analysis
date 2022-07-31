# Credit_Risk_Analysis
## Purpose 
The purpose of this analysis is to employ different techniques to train and evaluate models with Unbalanced classes by using imbalanced-learn and scikit-learn. For this challenge, I oversampled the credit data using RandomOverSampler and SMOTE. I also undersampled the data using the using the ClusterCentroids algorithm and SMOTEENN. Finally, I analysed the data and comared the two algorthms to predict credit risk. 


### Deliverable 1: Use Resampling Models to Predict Credit Risk
For Deliverable 1, I was tasked with evaulating three machine learning models by using resampling to determine if any of the models (RandomOverSampling, SMOTE, and CLusterCentroids) are better at determining credit risk.

#### RandomOverSampling Results
![Random_OverSampling](./Random_OverSampling.png)

#### SMOTE Results
![SMOTE_OverSampling](./SMOTE_OverSampling.png)

#### ClusterCentroid Results
![ClusterCentroid_UnderSampling](./ClusterCentroid_UnderSampling.png)

## Results
- Accuracy:
- Precision: The precision between all three models remained unaffected.
- Recall Score: The RandomOverSampling model had a mich higher score than SMOTE and the lowest recall score was from the ClusterCentroid with a recall score of 0.44


### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
For Deliverable 2, I used the combined approach of over and under-sampling with the SMOTEENN algorithm to determine if the if these results form a better approach at predicting the results from Deliverable 1.

#### SMOTEENN Results
![SMOTEEN_Over_Under_Sampling](./SMOTEENN_Over_Under_Sampling.png)

## Results
- Accuracy: 
- Precision: 
- Recall Score: 

### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
For Deliverable 3, I used the imblearn.ensemble library to train and compare two different classifiers (BalancedRandomForestClassifier, and EasyEnsembleClassifier) to predit credit risk.

#### BalancedRandomForestClassifier Results
![brfc_model](./brfc_model.png)

#### EasyEnsembleClassifier Results
![eec_model](./eec_model.png)

## Results
- Accuracy:
- Precision:
- Recall Scores:

## Summary 


## Resources 
- Jupyter Notebook
- Pandas
- mnlev
