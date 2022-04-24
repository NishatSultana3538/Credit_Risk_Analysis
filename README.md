# Credit_Risk_Analysis

## Background
Data preparation, statistical reasoning are some important component of  machine learning. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques need to be employed  to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries are used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we need to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we need to  use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we need to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally we need to evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.
## Resources:
## Results:
### Use Resampling Models to Predict Credit Risk:
Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.


Balanced accuracy scores
Precision 
Recall scores 

Accuracy Score: 
Precision High Risk: 
Precision Low Risk: 
Recall High Risk: 
Recall Low Risk: 

Accuracy
Precision
Recall
F1-Score

### Use the SMOTEENN algorithm to Predict Credit Risk:
### Use Ensemble Classifiers to Predict Credit Risk
#### Balanced Random Forest Classifier
#### Easy Ensemble AdaBoost Classifier

## Summary
