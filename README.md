# Credit_Risk_Analysis

## Background
Data preparation, statistical reasoning are some important component of  machine learning. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques need to be employed  to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries are used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we need to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we need to  use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we need to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally we need to evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.
## Resources:
## Results:
## Use Resampling Models to Predict Credit Risk:
Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Oversampling

#### Naive Random Oversampling

![NRM_ACC]()
![NRM-CL]()

Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

#### SMOTE Oversampling
![SMOTE_ACC]()
![SMOTE-CL]()


Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 



### Undersampling
![SMOTE_ACC]()
![SMOTE-CL]()
Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

### Combination (Over and Under) Sampling: Use the SMOTEENN algorithm to Predict Credit Risk:
![SMOTEEN_ACC]()
![SMOTEEN-CL]()
Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

## Use Ensemble Classifiers to Predict Credit Risk
#### Balanced Random Forest Classifier
![BRFC_ACC]()
![BRFC-CL]()
Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

#### Easy Ensemble AdaBoost Classifier
![EEAC_ACC]()
![EEAC-CL]()
Balanced accuracy scores: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

## Summary

All six credit risk analysis models show  low accuracy and recall scores . All of the models used here to perform the credit risk analysis show weak precision in determining if a credit risk is high. The last two models, the balanced random forest classifers and easy ensemble classifiers, show better results in almost all metrics compared to the other four models. The easy ensemble adaboost classifier has the highest accuracy and recall scores out of all the models which proves to show that it is the best machine learning model to utilize for our credit card analysis.
