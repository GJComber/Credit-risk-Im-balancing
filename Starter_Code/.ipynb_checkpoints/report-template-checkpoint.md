# Module 12 Analysis Report 


## This is a Credit Risk Modeling technique analysis.



### _Purpose of the analysis._

To compare several Machine learning models to determine which model performs the best in the task of identifying the risk of loan defaults.

### _Financial information used._
Looking at customer data from a lending company, it is focusing on 'loan status' to determine default risk amongst the companies customer base
 
### _Variable summary and output required._
The identified risk in this example is based on 'loan status' with a binary outcome of 'default' or 'not', hence a Logistic Regression model was chosen.
This is a popular classification algorithm that works well with binary outputs.

### _Stages of the machine learning analysis process._
* Read in the data
* Identify the target data and seperate it from the remaining dataset. 
* Evaluate the size of the dataset and degree of imbalance within it.
* Seperate the data into subsets comprising training and testing data.
* Model the data and train it using the training subset.
* Run predictions using the test subset.
* Evaluate the accuracy of the models predictions using several metrics methods.


### _Due to the inherently imbalanced nature of credit risk data, it is important to explore more than one method to determine the optimal model._
For a comparison model the data was then resampled with an added layer of random oversampling.
This is another process that can be overlayed onto the Logistic Regression model to mitigate the effects of imbalance within the dataset.
Essentially the training subset of data is made to be of equal amounts of target and reference data prior to training then running predictions on that.
Random oversampling increases the target data volume to be the same size as the reference data.
 
## Results


### _Machine Learning Model 1:_
  *  Model 1 Logistic Regression model.
  * Scores
  + Accuracy    0.9520479254722232,    
  + Precision   100% on safe loans and 85% on default loans, 
  + Recall       99% on safe loans and 91% on default loans.   



### _Machine Learning Model 2:_
  * Model 2 Logistic Regression model, resampled with Random Oversampling method.
  * Scores
  + Accuracy    0.9936781215845847,    
  + Precision   100% on safe loans and 84% on default loans, 
  + Recall       99% on safe loans and 99% on default loans. 
 
## Summary

Both models performed well but the oversampled model was a better choice.

The Precision is more important than the Recall when trying to identify and reduce default risk. 
The higher Specificity score is also important along with the higher Balanced Accuracy measure of the resampled model.

### _My Recommendation_
The adjusted  model was more accurate all round and where it was wrong it tended to err on the conservative side. Errors tended to be false negatives, with almost no false positives so for this business scenario I would recommend the Random Oversampled Logistic Regression model
