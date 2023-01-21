# credit-card-risk-Analysis

## *Overview of the analysis*
The intent of the project is to build a machine learning model to evaluate and predict risks associated with credit cards. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, the model uses techniques to train and evaluate models with unbalanced classes. In this project,  'imbalanced-learn' and 'scikit-learn' libraries are used to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data was oversampled using the 'RandomOverSampler' and 'SMOTE' algorithms, and undersample the data using the 'ClusterCentroids' algorithm. Next, two new machine learning models were compared that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## *Results*
* Naive Random Oversampling results: 
  - Balanced accuracy scores: 67%
  - Precision: 1%
  - Recall: 64%
  
![random_oversampling](https://github.com/AadiJan/credit-card-risk-Analysis/blob/a2787732fb1631d2cc35ae9796b45f050e7f0f3f/Random_oversampling.PNG)

* SMOTE oversampling results:
  - Balanced accuracy scores: 65%
  - Precision: 1%
  - Recall: 68%

![SMOTE_oversampling](https://github.com/AadiJan/credit-card-risk-Analysis/blob/a9649a41cb7d3a3fb311de68318e6d608139e7da/SMOTE_oversampling.PNG) 

* Undersampling results:
  - Balanced accuracy scores: 65%
  - Precision: 1%
  - Recall: 40%

![undersampling](https://github.com/AadiJan/credit-card-risk-Analysis/blob/8731c10fa0f9a47394a7e3128ba83caf14ac0933/Undersampling.PNG)

* Combination Results:
  - Balanced accuracy scores: 54%
  - Precision: 1%
  - Recall: 57%

![combination](https://github.com/AadiJan/credit-card-risk-Analysis/blob/b764e60b7701b702beb1ef2ece2ba820fb7565f4/Combination.PNG)

* Balanced Random Forest Classifier Results:
  - Balanced accuracy scores: 78%
  - Precision: 1%
  - Recall: 88%

![balanced-random](https://github.com/AadiJan/credit-card-risk-Analysis/blob/7b56ad8822736ea493a053883c4198a8dfe4e3f5/BalancedRandomForest_classifier.PNG)

* Easy Ensemble Classifier:
  - Balanced accuracy scores: 91%
  - Precision: 1%
  - Recall: 94%

![easy_ensemble](https://github.com/AadiJan/credit-card-risk-Analysis/blob/3ed3c976f8d7b88481409c6af019300955cc2ff1/Easy_ensemble.PNG)


## *Summary*
The models we undersampled, oversampled and a combination of both were used to determine the model that predicts as to which loans are at high risk. In addition to that, the last 2 models used emsemble classifiers to predict the high risk loans. The first four models had an accuracy of between 54% and 67%, which is quite low. However, using the easy ensemble had an highest accuracy of 91%. Therefore, I recommend using 'EasyEnsembleClassifier' model for this problem.
