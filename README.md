# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

The purpose of the project is to apply machine learning techniques to classify credit card risk into good loan (low risk) and bad loan (high risk) categories.

Credit risk is an unbalanced classification problem. That is, the proportion of good loans in the data is much higher than the proportion of bad loans. Training a model without adjusting for the imbalance in the data can lead to misleading results. For example, the model can have a very high overall accuracy score but is actually very poor at detecting bad loans. Several resampling techniques are explored to address the problem. 

First we oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier from the Imbalanced-Learn library, to predict credit risk. 

A credit card credit dataset from LendingClub, a peer-to-peer lending services company, is used for the analysis. The Imbalanced-Learn and Scikit-Learn libraries are used to resample data and to build and evaluate models. 



## Results

The accuracy, precision and recall scores are summarized for each of the six models:

![summary](summary.png)


Detailed classification report for each model:

- Oversampling using Naive Random Oversampling (ROS)

![ros_report](ros_report.png)


- Oversampling using SMOTE 

![smote_report](smote_report.png)


- Undersampling using Cluster Centroids (CC)

![cc_report](cc_report.png)


- Combination (Over and Under) sampling using SMOTEENN

![smoteenn_report](smoteenn_report.png)


- Balanced Random Forest Classifier (BRF)

![brf_report](brf_report.png)


- Easy Ensemble AdaBoost Classifier (EEC)
- 
![eec_report](eec_report.png)



## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


