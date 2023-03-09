# Credit_Risk_Analysis
Structure, Organization, and Formatting
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections (2 pt)
Each section has a heading and subheading (2 pt)
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis
The written analysis has the following:
## Overview:

We've been tasked with performing data preparation, statistical reasoning, and machine learning to assess credit card risk provided by the LendingClub, a peer-to-peer lending service. First, we'll load the `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models using resampling. Next, we'll oversample the data using `RandomOverSampler` and `SMOTE` algorithms. Third, we'll undersample the data using the `ClusterCentroids` algorithm. Then we'll oversample and undersample simultaneously with the `SMOTEENN` algorithm. Finally, we'll compare two new machine learning models that reduce bias: `BalancedRandomForestClassifier` and `EastEnsembleClassifier` to predict risk. Once we're done, we'll evaluate the performance of these models and assess which one should be used to predict credit risk.

## Results:

Random Over Sampler

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/random_oversampler.png)

- Balance Accuracy Score: 66%
- Precision: 99%
- Recall: 60%

SMOTE

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/smote.png)

- Balance Accuracy Score: 66%
- Precision: 99%
- Recall: 69%

Cluster Centroids

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/cc.png)

- Balance Accuracy Score: 54%
- Precision: 99%
- Recall: 40%

SMOTEENN

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/smoteenn.png)

- Balance Accuracy Score: 69%
- Precision: 
- Recall: 

Balanced Random Forest Classifier

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/Balanced_random_forest_classifier.png)

- Balance Accuracy Score: 79%
- Precision: 99%
- Recall: 87%

East Ensemble Classifier

![This is an image](https://github.com/aaron-ardell/Credit_Risk_Analysis/blob/main/pics/easy_ensemble_ada_boost_classifier.png)

- Balance Accuracy Score: 93%
- Precision: 99%
- Recall: 94%

## Summary

For the purpose of analysing credit risk, the most accurate machine learning process would be the first priority to weigh. The accuracy of the process will ensure the most accurate classifying of potential applicants as either high risk or low risk. Second, the sensitivity(recall) score, particularly when it comes to high


Overview of the loan prediction risk analysis:

The purpose of this analysis is well defined (4 pt)
Results:

Bullet points reviewing results
images of results

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
Summary:

There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
