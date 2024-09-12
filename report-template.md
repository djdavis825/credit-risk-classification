# Module 20 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* **Purpose of the analysis** - The goal of the analysis was to use the Logistic Regression machine learning model and determine if it could accurately predict healthy loans versus high risk loans.
* **The Dataset** - The analysis used a dataset of 77,536 loans. The dataset included columns for loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. **Loan_status** is the category that is being predicted in the analysis.
* **Stages of the Machine Learning Process** - The stages of machine learning directly provide an accurate calculation of the Logistic Regression machine learning models ability to make predictions. The stages included:

	* Prepare the data - Import the .csv file and made the DataFrame, analyze the outcomes
	* Separate the labels and features - Status of the loan labels were healthy (0) or high risk (1). Features of the remaining data use train and test model
	* Use the train_test_split function to sort labels and features into training and testing sets
	* Import model from the library - For this analysis, importing LogisticRegression from SKLearn
	* Instantiate the model
	* Fit model using training data
	* Use the model to make predictions
	* Evaluate the predictions - calculate and compare, ex: accuracy score, confusion matrix, classification report
* **Machine Learning Methods Utilized** - 
Primary model used:
	* LogisticRegression from SKLearn

	Supporting Functions:
	* train_test_split from SKLearn

	Evaluation tools:
	* from SKLearn:
		* confusion_matrix
		* classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model - Logistic Regression:
  * **Accuracy Score:** 99%
  * **Precision Scores:**
	  * Class 0 (Healthy Loans): 100%
	  * Class 1 (High Risk Loans): 85%
  * **Recall Scores:**
	  * Class 0 (Healthy Loans): 99%
	  * Class 1 (High Risk Loans): 91%

## Summary

Overall the model does well in predicting healthy and high risk loans.

Comparatively it does a better job predicting healthy loans than high risk loans. 
With healthy loans, precision was 100% and recall was 99%. While with high risk loans, precision was 85% and recall was 91%.

However the disparity in the occurrence of each type of loan should be considered as it still does a good job at predicting high risk loans.
