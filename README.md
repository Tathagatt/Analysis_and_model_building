## Analysis_and_model_building
## PROBLEM STATEMENT
The main aim of this project is to predict if the user would buy the product in the next 3 months or not based on various features which we will discuss as we go ahead.
## APPROACH
1.Data Analysis – 
•	I performed this step to understand more about the data like the shape of the data, the datatypes of different features.
•	After this used “isnull ()” operation to know which features have null values and if there is some relation between the null values and label using bar graph.
•	This operation provided me with insights that there is some relation and I imputed the null values with something meaningful so that the pattern can be found out by the model. 
•	Converted two ordinal features into categorical features by ranking then based on the label to improve accuracy.
•	Found out that one feature was away from the bell curve distribution so converted it into a Gaussian distribution using BOX-COX transformation as it was the best for the feature. 
2.Feature Engineering – 
•	Used the p-value for feature selection and LASSO regularization to decrease the complexity of the model. 
•	Used clustering algorithm too but it was not giving any good results.
3.Model Finder – 
•	Used Logistic Regression at first but the score was not good.
•	Then used Random Forest with some hyper parameters tuning and got the prediction where f1 score was good but not good enough. 
•	At last used XGBOOST Classifier with Stratified CV and got the best score in all the submission.
•	Tried all the models by balancing the data using RandomOverSampler but the results were not good so made the final model without balancing the dataset.

 
