# Credit_Risk_Analysis

## Python Code

[Credit Risk ensemble code](https://github.com/lindaxie7/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

[Credit Risk resampling code](https://github.com/lindaxie7/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)


## Overview of Project
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then, I evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


## Results

- Naive Random Oversampling results: balanced accuracy score is 50%, the precision is at 99% and the recall is 99%
![Untitled](https://user-images.githubusercontent.com/38533045/140630059-0bf818f4-110c-4bc6-9181-c22d6b3e0cd9.png)


- SMOTE oversampling results: balanced accuracy score is 63%, the precision is at 99% and the recall is 64%

![Untitled2](https://user-images.githubusercontent.com/38533045/140630086-57f7d058-d9ed-45cd-b807-a9b3b41885aa.png)


- Undersampling results: balanced accuracy score is 52%, the precision is at 99% and the recall is 41%

![Untitled3](https://user-images.githubusercontent.com/38533045/140630163-c58c8624-600c-40ee-80dc-1d4bfa94c7eb.png)

- Combination(over and undersampling) results: balanced accuracy score is 52%, the precision is at 99% and the recall is 57%

![Untitled4](https://user-images.githubusercontent.com/38533045/140630196-2f663d55-e9c4-450b-ad76-e3fd0da7802e.png)


- Balanced Random Forest Classifier results: balanced accuracy score is 99.6%, the precision is at 100% and the recall is 100%

![Untitled5](https://user-images.githubusercontent.com/38533045/140630255-0f61eba4-a22f-4146-b4b7-7d2f7f50c705.png)



- Easy Ensemble AdaBoost Classifier results: balanced accuracy score is 94.2%, the precision is at 99% and the recall is 94%

![Untitled6](https://user-images.githubusercontent.com/38533045/140630310-3fe0bc8e-653a-4172-a9d3-1b5cac3b69d3.png)



## Summary
 In the first four models the accuracy score is not as high as the ensemble classifiers, and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
