# Project 1: Bank Marketing Prediction

## 1) Project Overview

This project predicts whether a customer will subscribe to a term deposit (fixed deposit) based on their demographic details, financial information, and previous marketing campaign responses. It is a supervised machine learning classification problem with a clear business use case in banking.

## 2) Dataset Summary

* **Dataset Name:** Bank Marketing Dataset
* **Source:** UCI Machine Learning Repository
* **Type:** Structured tabular dataset
* **Target Variable:** `y` (yes/no)
* **Main Features:** age, job, marital status, education, default, housing, loan, contact, month, duration, campaign, pdays, previous, poutcome

## 3) Workflow

1. Load the dataset
2. Inspect data shape and distribution
3. Clean and preprocess the data
4. Encode categorical columns using One-Hot Encoding
5. Scale numerical columns
6. Split data into train and test sets
7. Train models such as Logistic Regression and Random Forest
8. Tune hyperparameters using GridSearchCV
9. Evaluate the model using accuracy, precision, recall, F1-score, and ROC-AUC

## 4) Key Result

The final model predicts whether a customer will subscribe to a term deposit with strong classification performance. This helps the bank focus only on likely customers and reduce unnecessary marketing effort.

## 5) Machine Learning Model

* **Baseline Model:** Logistic Regression
* **Main Model:** Random Forest Classifier
* **Tuning Method:** GridSearchCV

## 6) Association Rule

Association rule mining is not the main technique used in this project because the goal is classification. However, it can be used as an extension to find patterns such as which customer characteristics often appear together among subscribed customers.

## 7) Unique Thing About the Project

* Real-world banking use case
* Strong preprocessing and model comparison
* Can be extended with feature importance analysis

## 8) Viva Explanation Points

* This is a supervised learning classification project
* The output is binary: yes or no subscription
* Random Forest was chosen for better performance and reduced overfitting
* One-Hot Encoding was used for categorical variables
* Scaling was applied to numerical features
* The project helps banks improve campaign targeting and reduce cost

## 9) Good Viva Questions

1. Why is this a supervised learning problem?
2. Why did you choose Random Forest?
3. What is the difference between precision and recall?
4. Why is One-Hot Encoding needed?
5. Why did you use a pipeline?
6. What is overfitting?
7. What is ROC-AUC?
8. How does this project help banks in real life?
9. Why is train-test split important?
10. How can you improve the model further?

## Project Code Link

[https://colab.research.google.com/drive/1eb4ASFhl3bma3xP0luW9_6Unff-1G-xc?usp=sharing](https://colab.research.google.com/drive/1eb4ASFhl3bma3xP0luW9_6Unff-1G-xc?usp=sharing)

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab

## Final Note

This project shows how supervised machine learning can be used for customer prediction and business decision-making in banking.
