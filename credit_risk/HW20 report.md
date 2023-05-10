# Module 20 Report 

## Overview of the Analysis

In this analysis, a large dataset of loan information was used to build a prediction model to identify healthy loans vs unhealthy loans.  The dataset contained data on loan amount & interest rate as well as borrower information such as income, debt ratio, number of accounts, derogatory marks, and their total debt.  The result of the loan (healthy/unhealthy) was also in the data set which allowed us to use supervised learning models.  The data included information on 77,536 loans with 95% of the loans being healthy loans.

For the analysis, the dataset was split into a training set and then a set to test the model with.  A Logistic Regression model was built and analyzed.  Due to the imbalance in the type of loans in the dataset, oversampling was utilized and a second model created.  The second model yielded better results than the first.

## Results

* Machine Learning Model 1:
  * Healthy loans had a precision of 1.0, a recall of 0.99, and a combined f1-score of 1.00
  * Unhealthy loans had a precision of 0.85, a recall of 0.91, and a combined f1-score of 0.88
  * Balanced-accuracy for this model was 95.2%

* Machine Learning Model 2 (suing over-sampling):
  * Healthy loans had a precision of 1.0, a recall of 0.99, and a combined f1-score of 1.00
  * Unhealthy loans had a precision of 0.84, a recall of 0.99, and a combined f1-score of 0.91
  * Balanced-accuracy for this model was 99.4%

## Summary

Due to the extreme unbalance in the type of loans in the dataset, I would recommend using the 2nd model.  While both models do extremely well predicting the healthy loans, the 2nd model does a better job at having false negatives on the unhealthy loans (unhealthy loans that were actually predicted as healthy).  This is seen in the higher recall score for the unhealthy loans at nearly the same precision.  The overall model also had a high balanced-accuracy score.  

Ideally, additional data should be collected to provide the models with additional data to better predict the unhealthy loans and a third model created.
