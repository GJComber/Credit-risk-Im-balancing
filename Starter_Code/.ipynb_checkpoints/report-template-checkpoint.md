# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

 Credit risk modeling techniques using machine learning to identify the risk of loan defaults 

* Explain what financial information the data was on, and what you needed to predict.
Looking at customer data from a lending company focusing on 'loan status' to determine default risk amongst the companies customers
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The identified risk in this example is based on a binary outcome of default or no, hence a Logistic Regression model was chosen which is a popular classification algorithm 
* Describe the stages of the machine learning process you went through as part of this analysis.
The process is to read in the data, identify the target data and seperate it from the remaining dataset. It is then evaluated for degree of imbalance seperated into subsets comprising training and testing data then modelled and the accuracy of the models predictions are evaluated
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
 it was modelled with and without an added layer of random oversampling to compare methods for dealing with the imbalanced dataset.
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
for this we are using a logistic Regression model which is a classification algorithm


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
 Due to the inherently imbalanced nature of credit risk data, it is important to explore more than one method to determine the optimal model
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Given that the adjusted  model was more accurate all round and where it was  wrong it tended to err on the conservative side, IE errors tended to be false negatives, with almost no false positives so for this business scenario I would recommend the ROS model
