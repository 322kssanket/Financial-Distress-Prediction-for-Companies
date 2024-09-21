# Financial-Distress-Prediction-for-Companies
Problem Overview: 
This project focuses on predicting financial distress in companies using a combination of regression, classification, and clustering approaches. The dataset includes financial and non-financial features collected from sampled companies over varying time periods (1-14). The main objective is to classify companies as either financially distressed or healthy, based on the target variable "Financial Distress." If a company's financial distress value is greater than -0.50, the company is considered healthy (0), otherwise financially distressed (1).

The dataset is highly imbalanced, with 136 financially distressed companies compared to 286 healthy ones (or 136 firm-year observations versus 3546 healthy firm-year observations). Due to this imbalance, we emphasize using f-score, Precision, Recall, and F1-Score as performance evaluation metrics for classification tasks. Additionally, 30% of the dataset will be used as a hold-out test set, while the remaining 70% will be used for feature selection and model training.

Dataset Structure
Company: Represents the companies in the sample.
Time: Denotes the different time periods associated with each company.
Financial Distress: The target variable; if greater than -0.50, the company is considered healthy (0), otherwise distressed (1).
x1 to x83: Financial and non-financial characteristics of companies used as features. Feature x80 is categorical.
Tasks:
1. Regression:
We perform regression on one of the numerical attributes to predict financial performance. The following regression models are implemented:

Logistic Regression
Random Forests
Extra Random Trees
AdaBoost
Evaluation metrics include:Root Mean Squared Error (RMSE), Mean Absolute Error (MAE)

2. Classification:
Using the "Financial Distress" label, we classify companies as either healthy or financially distressed. The following classification algorithms are implemented:
Naive Bayes,
K-Nearest Neighbors (KNN),
Support Vector Machines (SVM),
Decision Trees
Evaluation metrics include: Precision, Recall, F1-Score

3. Clustering:
Clustering is applied to group companies based on all available attributes, aiming to uncover patterns in the data. The following clustering techniques are used:
K-Means (with appropriate k),
EM Clustering,
K-Medoids
The Sum of Squared Errors (SSE) is computed for each clustering output to evaluate the performance.

Getting Started
Prerequisites
Python 3.x
Libraries: scikit-learn, numpy, matplotlib, pandas
