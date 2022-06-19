# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

The purpose of the project is to apply machine learning techniques to classify credit card risk into good loan (low risk) and bad loan (high risk) categories.

Credit risk is an unbalanced classification problem. That is, the proportion of good loans in the data is much higher than the proportion of bad loans. Training a model without adjusting for the imbalance in the data can lead to misleading results (the model can have a very high overall accuracy score but is very poor at detecting the bad loans). Several resampling techniques were explored to address the problem. 

A credit card credit dataset from LendingClub, a peer-to-peer lending services company, is used for the analysis. The Imbalanced-Learn and Scikit-Learn libraries are used to resample data and to build and evaluate models. 

you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

1. Oversampling using Naive Random Oversampling

Balanced accuracy score = 0.6456130066757718

![ros_report](ros_report.png)

2. Oversampling using SMOTE 

Balanced accuracy score = 0.6234433606890912

![smote_report](smote_report.png)


3. Undersampling using Cluster Centroids 

Balanced accuracy score = 0.5138873780775228

![cc_report](cc_report.png)

4. Combination (Over and Under) sampling using SMOTEENN

Balanced accuracy score = 0.6156536172852936

![smoteenn_report](smoteenn_report.png)

5. Balanced Random Forest Classifier (Imbalanced-Learn)

Balanced accuracy score = 0.7885466545953005

![brf_report](brf_report.png)

6. Easy Ensemble AdaBoost Classifier (Imbalanced-Learn)

Balanced accuracy score = 0.9316600714093861

![eec_report](eec_report.png)

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


