# Customer Churn Prediction Project Report

## Introduction

This project aims to predict customer churn for a telecom company using data analysis and machine learning techniques. Customer churn is a critical metric for businesses as it measures the rate at which customers stop using their services. Identifying and understanding the factors that contribute to customer churn can help the company take proactive measures to retain customers and improve their overall business performance.

In this report, we will provide an overview of the project, the data used, the analysis performed, and the machine learning models developed to predict customer churn.

## Data

The dataset used in this project was sourced from an Excel file named "data.xlsx." The dataset contains information about various customers, including their demographics, usage patterns, billing information, and whether they churned or not. Here's a brief description of the columns in the dataset:

- `age`: Customer's age
- `gender`: Customer's gender
- `location`: Customer's location
- `months`: Number of months as a customer
- `bill`: Billing information
- `usage`: Usage patterns
- `churn`: A binary variable indicating whether the customer churned (1) or not (0)

The data exploration and preprocessing steps included handling missing values, grouping usage into quarters, and converting categorical variables into factors. Exploratory Data Analysis (EDA) was also conducted to understand the distribution and relationships between variables.

## Analysis

### Logistic Regression

We started by splitting the data into training and testing sets (70% training, 30% testing) and fitting a logistic regression model. The logistic regression model helped us understand the relationship between independent variables and customer churn. We assessed the model's accuracy and examined feature importance through the odds ratios.

### Decision Tree

We also employed a decision tree classifier to predict customer churn. The decision tree was visualized for better interpretation, and its accuracy was assessed on both the training and testing datasets.

### Random Forest

A random forest classifier was used to predict customer churn, initially with default hyperparameters. The model's performance was evaluated, and feature importance was determined. Hyperparameter tuning was performed to optimize the random forest model further.

## Results

### Logistic Regression Results

- Logistic Regression Accuracy: 79.2%
- Confusion Matrix:
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

### Decision Tree Results

- Decision Tree Accuracy: 76.5%
- Confusion Matrix:
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

### Random Forest Results

- Random Forest Accuracy (Default Hyperparameters): 85.3%
- Random Forest Accuracy (Tuned Hyperparameters): 86.1%
- Confusion Matrix (Tuned Hyperparameters):
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

## Conclusion

In this customer churn prediction project, we explored, preprocessed, and analyzed customer data to develop machine learning models for predicting churn. The random forest model with tuned hyperparameters achieved the highest accuracy of 86.1%, outperforming both logistic regression and decision tree models.

Understanding the factors contributing to customer churn is vital for businesses to take proactive measures to retain their customers. By using the insights gained from this analysis and predictive modeling, the telecom company can develop strategies to reduce customer churn, ultimately leading to improved customer satisfaction and profitability.

The code and documentation for this project can be found in the GitHub repository R-Code.
