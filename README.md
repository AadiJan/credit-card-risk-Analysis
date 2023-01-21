# credit-card-risk-Analysis

## *Overview of the analysis*
The intent of the project is to build a machine learning model to evaluate and predict risks associated with credit cards. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, the model uses techniques to train and evaluate models with unbalanced classes. In this project,  'imbalanced-learn' and 'scikit-learn' libraries are used to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data was oversampled using the 'RandomOverSampler' and 'SMOTE' algorithms, and undersample the data using the 'ClusterCentroids' algorithm. Next, two new machine learning models were compared that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## *Results*
* Naive Random Oversampling results: 
Balanced accuracy scores: 67%
Precision: 1%
Recall: 64%
![random_oversampling](https://github.com/AadiJan/credit-card-risk-Analysis/blob/a2787732fb1631d2cc35ae9796b45f050e7f0f3f/Random_oversampling.PNG)

* SMOTE oversampling results:
Balanced accuracy scores:
Precision: 1%
Recall: 64%
