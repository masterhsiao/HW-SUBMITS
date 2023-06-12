# Module 12 Report
Overview of the Analysis
In this analysis, we developed machine learning models to predict small business loan defaults. The dataset contained financial information about the loans, and our task was to predict the loan status.

## We followed these steps:

- Data Preprocessing: Separated the data into features and labels and performed train-test split. Checked the balance of target values.

- Model Training and Evaluation: Trained a Logistic Regression model on the original data and evaluated its performance using classification metrics.

- Addressing Imbalanced Data: Used RandomOverSampler to oversample the minority class. Trained another Logistic Regression model on the oversampled data and evaluated its performance.

# Results
##Logistic Regression Model (Original Data):

Balanced Accuracy: 0.952

Precision, Recall, F1-Score (Default Class): 0.85, 0.91, 0.88

Precision, Recall, F1-Score (Non-default Class): 1.00, 0.99, 1.00

##Logistic Regression Model (Oversampled Data):

Balanced Accuracy: 0.995

Precision, Recall, F1-Score (Default Class): 0.99, 0.99, 0.99

Precision, Recall, F1-Score (Non-default Class): 0.99, 0.99, 0.99

# Summary
The Logistic Regression model trained on the oversampled data outperformed the model trained on the original data. It achieved a balanced accuracy of 0.995 and demonstrated high precision, recall, and F1-score for both default and non-default classes.

We recommend using the Logistic Regression model trained on the oversampled data for predicting loan defaults. However, the choice of model should consider the specific problem requirements, such as prioritizing recall for the minority class or achieving high precision for the non-default class.
