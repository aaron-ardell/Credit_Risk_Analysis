# Credit_Risk_Analysis

## Overview:

We've been tasked with performing data preparation, statistical reasoning, and machine learning to assess credit card risk provided by the LendingClub, a peer-to-peer lending service. First, we'll load the `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models using resampling. Next, we'll oversample the data using `RandomOverSampler` and `SMOTE` algorithms. Third, we'll undersample the data using the `ClusterCentroids` algorithm. Then we'll oversample and undersample simultaneously with the `SMOTEENN` algorithm. Finally, we'll compare two new machine learning models that reduce bias: `BalancedRandomForestClassifier` and `EastEnsembleClassifier` to predict risk. Once we're done, we'll evaluate the performance of these models and assess which one should be used to predict credit risk.

## Results:

### Random Over Sampler

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/random_oversampler.png)

- Balance Accuracy Score: 66%
- Precision: 99%
- Recall: 60%

### SMOTE

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/smote.png)

- Balance Accuracy Score: 66%
- Precision: 99%
- Recall: 69%

### Cluster Centroids

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/cc.png)

- Balance Accuracy Score: 54%
- Precision: 99%
- Recall: 40%

### SMOTEENN

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/smoteenn.png)

- Balance Accuracy Score: 69%
- Precision: 99%
- Recall: 60%

### Balanced Random Forest Classifier

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/Balanced_random_forest_classifier.png)

- Balance Accuracy Score: 79%
- Precision: 99%
- Recall: 87%

### East Ensemble Classifier

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/easy_ensemble_ada_boost_classifier.png)

- Balance Accuracy Score: 93%
- Precision: 99%
- Recall: 94%

## Summary

There are a series of criteria to meet to determine the best overall machine learning process for identifying credit risk. First, the Balance Accuracy Score will provide us a glimpse at how reliable our model is performing. Second, the recall(sensitivty) particularly concerning the high risk status of applicants. For this application, it's far better to identify all of the high risk applicants even if that means more low risk applicants are mis-identified as high risk. This way our client does not issue loans to applicants that are unable to repay.

Balance Accuracy Score: 
- East Ensemble Classifier: 93%
- Balanced Random Forest Classifier: 79%
- SMOTEENN: 69%

Recall: 
- East Ensemble Classifier: 94%
- Balanced Random Forest Classifier: 87%
- SMOTE: 69%

The East Ensemble ADA Boost Classifier scored very good in Balanced Accuracy Score and over all Recall. It also had the highest sensitivty rate for the high risk applicants at 92%. This machine learning process would be the best for identifying credit risk for our client, the Lending Club.
