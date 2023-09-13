# credit-risk-classification-challenge20

Overview of analysis 
•	The purpose of this analysis was to create and evaluate a supervised machine learning model that would predict the credit worthiness of potential borrowers: by identifying if a loan was healthy or high-risk. 
•	The data used was a 77,536-line csv file that contained columns of various data about the loan (amount and interest rate) and the borrower's income, debt and accounts, as well as a column classifying the loan as healthy or high-risk. 

To perform the machine learning process the data was:
1.	Split into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
2.	Then split the data into training and testing data sets.
3.	A Logistic Regression model from sklearn was created with the Limited-memory BFGS ('lbfgs') solver. As we are classifying loans as either healthy OR high-risk, with only these two as options Logistic Regression was chosen. 
4.	The model was then fit with the training data.
5.	Predictions were made with the test data.
6.	The model was evaluated by comparing the predictions with the test labels.

Results 

Machine learning model 1:
 These metrics for class 0 are excellent. The precision of 1.00 indicates that almost all predictions for healthy loans are correct, and the recall of 0.99 shows that the model captures nearly all of the actual healthy loans. The F1-score of 1.00 is a harmonic mean of precision and recall, and it's also very high.
These metrics for class 1 are also good. The precision of 0.85 means that about 85% of the predicted high-risk loans are correct, and the recall of 0.91 suggests that the model captures 91% of the actual high-risk loans. The F1-score of 0.88 indicates a good balance between precision and recall for class 1.
Overall, the logistic regression model performs exceptionally well for class 0 (healthy loans) with very high precision, recall, and F1-score. It also performs reasonably well for class 1 (high-risk loans) with good precision, recall, and F1-score. These metrics suggest that the model is effective at distinguishing between healthy and high-risk loans, with a high degree of accuracy and reliability.

Machine learning model 2:	
The metrics for class 0 indicate that the model correctly identifies almost all healthy loans (class 0) with very high precision, recall, and F1-score.
For class 1 (high-risk loans), the model also performs exceptionally well, with high precision, recall, and F1-score. This means that the model correctly identifies almost all high-risk loans with very few false positives.
Overall the logistic regression model predicts the oversampled data with a near-perfect accuracy (>99% accurate).

Summary 
In summary, both model 1 and model 2 exhibit exceptional performance with very similar metrics. They have high precision, recall, and F1-scores for both classes, indicating their effectiveness in distinguishing between healthy and high- risk loans. The choice between these models should be bases on practical considerations, as their performance metrics are very similar. 
