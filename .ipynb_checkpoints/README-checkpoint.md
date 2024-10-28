# credit-risk-classification
Module 12 Report

Overview of the Analysis

In this analysis, the objective was to assess the credit risk of loans using machine learning techniques. Specifically, we aimed to predict whether a loan was likely to default based on financial information from the dataset, using a classification approach.

Data Information: The dataset contained various financial attributes related to individual loans, with the target variable loan_status indicating the loan's status (e.g., default or non-default).

Objective: We needed to predict the likelihood of a loan defaulting, classified as 1 (default) or 0 (non-default). By examining loan_status, we could determine the distribution of defaults and non-defaults in the data.

Machine Learning Process:

Data Preparation: The data was divided into features (X) and labels (y), followed by a train-test split to enable performance evaluation on unseen data.

Model Selection: A LogisticRegression model was chosen.

Training: The model was trained on the training dataset.

Evaluation: The model’s performance was measured using accuracy, precision, and recall metrics on both training and test data.

Results

Below are the accuracy, precision, and recall scores from the LogisticRegression model:

Machine Learning Model 1 (Logistic Regression):

- Testing Accuracy: Approximately 99.6%, which means that this model is very accurate

- Precision and Recall:
For the healthy loan class (0):
Precision: very High at a perfect score of 100%, indicating strong identification of non-defaults.
Recall: very High at a perfect score of 100%, suggesting few actual non-defaults were missed.

For the high-risk loan class (1):
Precision: Lower than for the healthy loan class, indicating a greater chance of false positives.
Recall: Moderate, showing some defaults were missed.

Summary


I would recommend The LogisticRegression model because it achieved high accuracy in predicting loan defaults and has a great precision-recall balance.

Healthy loan (0) performed best because its precision and recall was perfect at 100%. However, high-risk loans performed well too. The numbers just show that it's able to predict high-risk loans for the most part.

Yes, performance does depend on the problem we're trying to solve. If minimizing financial losses is what's important here, then having a model that has a higher recall and precision for high-risk loans (1) would be more important. It depends on what the goal is here. If predicting high-risk loans (1s) is a priority, increasing the recall for high-risk loans might be advisable, possibly through further tuning or experimenting with other classification models.