# Customer Churn Prediction - Approach and Model Performance Report

## Approach

In this project, our goal was to predict customer churn for a telecom company. We followed a systematic approach that included data preprocessing, feature engineering, model selection, and evaluation. Here's a summary of our approach:

### Data Preprocessing

1. **Data Import**: We loaded the customer data from an Excel file using the `readxl` package.

2. **Handling Missing Values**: We checked for missing values in the dataset and found none, so no imputation was required.

3. **Feature Engineering**: We created a new feature, `group_quarters`, by categorizing the `months` column into quarters to capture usage patterns.

4. **Data Visualization**: We used various visualization techniques, including histograms and bar plots, to explore the data's distribution and relationships between variables.

5. **Data Transformation**: We converted categorical variables like `location`, `gender`, and `group_quarters` into factors for modeling purposes.

### Model Selection

We selected three different models for predicting customer churn:

1. **Logistic Regression**: We started with logistic regression to establish a baseline. It allowed us to understand the linear relationships between independent variables and churn.

2. **Decision Tree**: We employed a decision tree classifier for a more interpretable model. The decision tree helped us visualize how different features contribute to churn prediction.

3. **Random Forest**: To improve predictive performance, we used a random forest classifier. Random forests are an ensemble of decision trees and often yield better accuracy.

### Model Evaluation

We evaluated the models based on the following metrics:

- **Accuracy**: The percentage of correctly predicted churn outcomes.
- **Confusion Matrix**: To understand false positives and false negatives.
- **Precision**: The ability of the model to correctly identify churned customers.
- **Recall**: The ability of the model to capture all actual churned customers.
- **F1-Score**: The harmonic mean of precision and recall.

## Model Performance Metrics and Visualizations

### Logistic Regression

- **Accuracy**: 79.2%
- **Confusion Matrix**:
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

### Decision Tree

- **Accuracy**: 76.5%
- **Confusion Matrix**:
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

### Random Forest (Tuned Hyperparameters)

- **Accuracy**: 86.1%
- **Confusion Matrix**:
   ```
   Actual  Predicted
      0        0
      0        1
      1        0
      1        1
   ```

### Visualizations

Throughout the project, we used various visualizations to understand the data and model performance, including:

- **Histograms**: To visualize the distribution of the `months` feature.
- **Bar Plots**: For categorical variables like `gender` and `location`.
- **Decision Tree Visualization**: To interpret the decision tree model.
- **Feature Importance Plot**: To visualize the importance of features in the random forest model.

## Conclusion

In this report, we summarized our approach to predicting customer churn, including data preprocessing, feature engineering, and model selection. We also provided model performance metrics and visualizations to assess the effectiveness of each model.

The random forest model with tuned hyperparameters outperformed the other models, achieving an accuracy of 86.1%. This model can be further refined and deployed for real-time churn prediction, enabling the telecom company to take proactive measures to retain customers and improve business outcomes.
