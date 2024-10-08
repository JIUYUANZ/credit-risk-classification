### Credit-risk-classification challenge

## An overview of the analysis

The purpose of this analysis is to establish a predictive assessment model based on factors such as loan amount, interest rate, borrower income, and so on. The dependent variable (y value) in this analysis is the `loan status`, which indicates whether a loan is healthy or at risk. The independent variables (x values) include `loan size`, `interest rate`, `borrower income`, `number of accounts`, `derogatory marks`, and `total debt`.

Initially, I separated the data into labels and features, then performed a `train_test_split` split the data. I established a Logistic Regression model. Finally, I built the predictive model using the `X_test` data and calculated the accuracy to understand the model's balance.

## The results

In the “loan_status” column, '0' means that the loan is healthy, and 1 means that the loan has a high risk of defaulting. 

* Accuracy Score:
   * Achieved an accuracy of 99%.
   * Indicates that the model correctly predicts 99% of all samples.
* Precision Score:
   * Precision for healthy loan: 1.00 (100%), meaning all predicted healthy loans are indeed healthy.
   * Precision for high-risk loan : 0.84 (84%), indicating that 84% of the predicted high-risk loans are actually high-risk.
* Recall Score:
   * Recall for healthy loan: 0.99 (99%), showing that 99% of actual healthy loans were correctly identified.
   * Recall for high-risk loan: 0.94 (94%), suggesting that 94% of actual high-risk loans were correctly predicted.


## Summary

According to the classification report, we could see that the model performs well with 99% overall accuracy. That means most predictions are correct. But the precision for high risk loan is relatively low. That probably caused by small number of samples which is 619. In conclusion, the model performs excellently for healthy loans, but there is room for improvement in predicting high-risk loans.