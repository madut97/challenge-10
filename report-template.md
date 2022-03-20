# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to determine the accuracy and precision of machine learning models in identifying healhty and risky loans. 
* The financial infomration we used for the analysis was lending data located in the lending_data.csv file, which provides data for factors including: loan size, interest rate, borrower income, debt to income, # of accounts, derogatory marks and total in debt which are used in determining the "healthiness" of a loan, also indicated by the loan_status column, which our models look to predict. 
* The variable we were trying to predict was the loan_status column, using all other columns as the features/training features. Furtheremore, we used the value_counts function to calculate the numbebr of healhty and risky loans in the given data set. 
* Stages followed:
  * Stage 1: Upload the data
  * Stage 2: Separate the data into features/X (in this case everything excluding loan status) and labels/y (loan status).
  * Stage 3: Check the balance for the label.
  * Stage 4: Split the data into training and testing datasets by using `train_test_split` function. 
  * Stage 5: Fit the the logistic regression model using trained Xs and ys, and then make predictions for y using the logistic_regression_model functionality. 
* The prediction method used for both models was logitstic regression, with the differentiator being the usage of resampling for Model 2.  

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
      * Accuracy score: ~95%
      * Precision score: 
          * 0: 1.00 
          * 1: 0.85
      * Recall score: 0.99

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
      * Accuracy score: ~99%
      * Precision score:
          * 0: 1.00 
          * 1: 0.84
      * Recall score: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
    * Given that the precision score for predicting 0's (healthy loans) is same for both Model 1 & 2, and that there is only a minor difference in precision for predicting 1's (risky loans) is minor, both the higher accuracy score and higher recall score makes Model 2 the better performer, in my opinion. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
    * Given that the aim of this model is identifying risky loans, predictig 1`s is more important. 

If you do not recommend any of the models, please justify your reasoning.
