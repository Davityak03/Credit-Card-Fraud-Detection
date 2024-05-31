# Credit-Card-Fraud-Detection

# Credit Card Fraud Detection

This project uses the `creditcard.csv` dataset to detect fraudulent credit card transactions. The dataset contains transactions made by credit cards in September 2013 by European cardholders. The project implements machine learning algorithms such as Logistic Regression and Naive Bayes for fraud detection.

## Overview

The `creditcard.csv` dataset contains transactions over two days, with 492 frauds out of 284,807 transactions. The dataset is highly imbalanced, with the positive class (frauds) accounting for only 0.172% of all transactions.

## Dataset

The dataset has 31 columns, each representing a different feature of the transactions. Here are the key columns:

- **Time**: The elapsed time in seconds between this transaction and the first transaction in the dataset.
- **V1, V2, ..., V28**: Principal components obtained using PCA (Principal Component Analysis). Due to confidentiality issues, the original features are not provided, and these are the transformed features.
- **Amount**: The transaction amount.
- **Class**: The response variable, taking value 1 in case of fraud and 0 otherwise.
The dataset has been taken from kaggle

## Machine Learning Algorithms

### Logistic Regression

Logistic Regression is a linear model for binary classification. It predicts the probability of a binary outcome using a logistic function. The logistic function outputs values between 0 and 1, which can be interpreted as probabilities. Logistic Regression is widely used for binary classification problems due to its simplicity and effectiveness.

Advantages:
- Simple to implement and interpret.
- Can handle large datasets.
- Provides probabilities of class membership.

Disadvantages:
- Assumes a linear relationship between the features and the log odds of the outcome.
- Not effective for non-linear problems without feature engineering.

### Naive Bayes

Naive Bayes is a probabilistic classifier based on Bayes' Theorem with the assumption of independence between features. It calculates the probability of each class given the input features and selects the class with the highest probability. Despite the independence assumption, Naive Bayes performs well in many real-world applications, especially for text classification.

Advantages:
- Simple and fast.
- Works well with high-dimensional data.
- Requires a small amount of training data.

Disadvantages:
- Assumes independence between features, which is often not true in real-world data.
- Sensitive to the distribution of the features.

## Project Structure

- `data/`: Contains the `creditcard.csv` dataset.
- `notebooks/`: Jupyter notebooks used for data exploration and model training.
- `scripts/`: Python scripts for data preprocessing, training models, and evaluation.
- `results/`: Contains model performance metrics and visualizations.
- `README.md`: Project overview and instructions.


