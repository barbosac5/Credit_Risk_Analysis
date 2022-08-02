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
  - RandomOverSampling had a score of 0.65
  - SMOTE had a score of 0.64
  - ClusterCentroid had teh lowest score of 0.53
- Precision: 
  - RandomOverSampling: High Risk precision is low; Low Risk precision is high
  - SMOTE: High Risk precision is low; Low Risk precision is high
  - ClusterCentroid: High Risk precision is lowl Low Risk precision is high
              
- Recall Score: 
  -  The recall score between all three models are as follows:
              - RandomOverSampling: High Risk is 0.62; Low Risk is 0.68
              - SMOTE: High Risk is 0.63; Low risk is 0.66
              - ClusterCentroid: High Risk and low risk is the lowest of the three being 0.59 and 0.44 respectiely 
  - The RandomOverSampling model had a mich higher score than SMOTE and the lowest recall score was from the ClusterCentroid with a recall score of 0.44


### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
For Deliverable 2, I used the combined approach of over and under-sampling with the SMOTEENN algorithm to determine if the if these results form a better approach at predicting the results from Deliverable 1.

#### SMOTEENN Results
![SMOTEEN_Over_Under_Sampling](./SMOTEENN_Over_Under_Sampling.png)

## Results
- Accuracy: The accuracy of the SMOTEENN model is 0.64
- Precision: The precision for high risk is low and the low risk precision is high
- Recall Score: 
  - The high risk score is 0.70
  - The low risk score is 0.57

### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
For Deliverable 3, I used the imblearn.ensemble library to train and compare two different classifiers (BalancedRandomForestClassifier, and EasyEnsembleClassifier) to predit credit risk.

#### BalancedRandomForestClassifier Results
![brfc_model](./brfc_model.png)

#### EasyEnsembleClassifier Results
![eec_model](./eec_model.png)

## Results
- Accuracy: 
  - EasyEnsemble model scored the highest with 0.92 
  - BalancedRandomForestClassifier had a score of 0.79
- Precision:
  - The High Risk precision for BalancedRandomForestClassifier is low and the low risk is high
  - The High Risk precision for EasyEmsemble is low and the low risk is high
- Recall Scores: 
  - The high risk score for BalancedRandomForestClassifier is low and the low risk is high 
  - The high risk score for EasyEmsemble is high and the low risk is high

## Summary 
Out of all six models we worked with, I think the best model is the EasyEnsembleClassifier model first simply due to the fact that it scoared above 90% for the accuracy.  The other models has a much lower accuracy with the second hight being around 0.80. The precision between all the models were relatively similar. The recall score for the EasySemsembleClassifier was the best with both the low risk and high risk being in the 0.90 range. The randomOverSampling, SMOTE, and ClusterCentroid models do not even compete with the EasyEnsembleClassifier due to the fact that the highest scores with those three models were in the 0.50 - 0.65 range overall. The best model to use to determine credit risk would easily be the EasyEmsenbleClassifer model.

## Resources 
- Jupyter Notebook
- Pandas
- mnlev
