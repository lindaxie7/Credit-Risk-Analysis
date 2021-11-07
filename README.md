# Credit_Risk_Analysis

## Overview of Project
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then, I evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


## Results

- Naive Random Oversampling results: balanced accuracy score is 50%, the precision is at 99% and the recall is 99%
![Untitled](https://user-images.githubusercontent.com/38533045/140629997-035b0c79-c1cd-4f7a-b26a-7aed395eef0b.png)

- SMOTE oversampling results: balanced accuracy score is 63%, the precision is at 99% and the recall is 64%
![Untitled2](https://user-images.githubusercontent.com/38533045/140630005-3d1f0d66-246a-4a1f-9661-195b7bd7b3f8.png)

- Undersampling results: balanced accuracy score is 52%, the precision is at 99% and the recall is 41%

- Combination(over and undersampling) results: balanced accuracy score is 52%, the precision is at 99% and the recall is 57%

- Balanced Random Forest Classifier results: balanced accuracy score is 99.6%, the precision is at 100% and the recall is 100%

- Easy Ensemble AdaBoost Classifier results: balanced accuracy score is 94.2%, the precision is at 99% and the recall is 94%



## Summary
 In the first four models the accuracy score is not as high as the ensemble classifiers, and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
