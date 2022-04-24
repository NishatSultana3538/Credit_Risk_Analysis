# Credit_Risk_Analysis

## Background
Data preparation, statistical reasoning are some important component of  machine learning. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques need to be employed  to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries are used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we need to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we need to  use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we need to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally we need to evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.
## Resources:
Data Source: LoanStats_2019Q1.csv [LoanStats]()
Software: Python 3.8.3 , Jupyter Notebook 
## Results:
## Use Resampling Models to Predict Credit Risk:
Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Oversampling

#### Naive Random Oversampling

![NRM_ACC](https://github.com/NishatSultana3538/Credit_Risk_Analysis/blob/main/Image/NRO%20ACC.png)
![NRM-CL](https://github.com/NishatSultana3538/Credit_Risk_Analysis/blob/main/Image/NRO%20CL.png)

* Balanced accuracy scores: 65%
* Precision High Risk: 1%
* Precision Low Risk: 99%
* Recall High Risk: 62%
* Recall Low Risk: 68%

#### SMOTE Oversampling
![SMOTE_ACC](https://github.com/NishatSultana3538/Credit_Risk_Analysis/blob/main/Image/SMOTE%20ACC.png)
![SMOTE-CL](https://github.com/NishatSultana3538/Credit_Risk_Analysis/blob/main/Image/SMOTE%20CL.png)


* Balanced accuracy scores: 64%
* Precision High Risk: 1%
* Precision Low Risk: 99%
* Recall High Risk: 63%
* Recall Low Risk: 66%



### Undersampling
![CC_ACC]()
![CC-CL]()
* Balanced accuracy scores: 53%
* Precision High Risk: 1%
* Precision Low Risk: 99%
* Recall High Risk: 61%
* Recall Low Risk: 45%

### Combination (Over and Under) Sampling: Use the SMOTEENN algorithm to Predict Credit Risk:
![SMOTEEN_ACC]()
![SMOTEEN-CL]()
* Balanced accuracy scores: 62%
* Precision High Risk: 1%
* Precision Low Risk: 99%
* Recall High Risk: 68%
* Recall Low Risk: 57%

## Use Ensemble Classifiers to Predict Credit Risk
#### Balanced Random Forest Classifier
![BRFC_ACC]()
![BRFC-CL]()
* Balanced accuracy scores: 79%
* Precision High Risk: 3%
* Precision Low Risk: 97%
* Recall High Risk: 70%
* Recall Low Risk: 87%

#### Easy Ensemble AdaBoost Classifier
![EEAC_ACC]()
![EEAC-CL]()
* Balanced accuracy scores: 93%
* Precision High Risk: 9%
* Precision Low Risk: 91%
* Recall High Risk: 92%
* Recall Low Risk: 94%

## Summary
In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are at risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk.

In our first four models, we got weak precision, accuracy and recall scores in determining if a credit risk is high. The last two Ensemble models, the balanced random forest classifers and easy ensemble classifiers, show better results in almost all metrics compared to the other four models. The easy ensemble adaboost classifier has the highest accuracy and recall scores out of all six models which proves to show that it is the best machine learning model to utilize out of all six models.

Typically in our models, we want a good balance of recall and precision which is why I recommend the ensemble classifiers over the Resampling models. It appears that the Easy Ensemble Adaboost Classifier has high accuracy score and good balance of precision and recall scores so I will recommend this model out of all six models.

