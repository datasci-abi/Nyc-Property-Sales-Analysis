# NYC Property Sales Price Prediction

## Overview

This project focuses on predicting property sale prices in New York City using advanced machine learning models such as Linear Regression and XGBoost. Utilizing the NYC Citywide Rolling Calendar Sales dataset, this project entails cleaning data, building and evaluating models, and interpreting the results using advanced techniques like SHAP and Partial Dependence Plots.

## Dataset

The dataset includes details about property sales in NYC, with features such as:

- Neighborhood
- Building Class
- Land Square Feet
- Gross Square Feet
- Year Built
- Sale Price

## Key Steps

### Data Preprocessing

- Clean data by removing rows with missing values and converting text-based numbers (e.g., "1,000") to numeric format.
- Apply preprocessing pipelines for numerical and categorical data using `sklearn`.

### Data Visualization

- **Histogram**: Visualizes the distribution of Sale Prices.
- **Scatter Plot**: Examines the relationship between Gross Square Feet and Sale Price.

### Model Training

- **Linear Regression**: Serves as a simple baseline model.
- **XGBoost**: Advanced model aimed at improving prediction accuracy.

### Model Evaluation

- Evaluate models using metrics such as MAE (Mean Absolute Error), RMSE (Root Mean Squared Error), and R² Score.

### Feature Importance

- **Permutation Importance**: Identify which features most significantly impact model performance.

### SHAP Analysis

- Utilize SHAP (SHapley Additive exPlanations) to explain individual predictions and understand global feature importance.

## Results

- **Linear Regression**:
  - MAE: 1,220,872
  - RMSE: 7,550,325
  - R²: 0.07
- **XGBoost**:
  - MAE: 1,112,774
  - RMSE: 7,552,393
  - R²: 0.07

XGBoost performed slightly better than Linear Regression in terms of MAE and RMSE.

## Visualizations

- **Partial Dependence Plot (PDP)**: Demonstrates how features like Gross Square Feet influence predictions.
- **SHAP Plots**: Visualize feature importance and the decision-making process for individual predictions.

## Installation

Install the required libraries by running:

```bash
pip install pandas matplotlib scikit-learn xgboost shap pdpbox joblib
Usage
To run this project:

Preprocess the dataset using the provided preprocessing pipelines.
Train the models (Linear Regression and XGBoost).
Evaluate the models using the specified metrics.
Analyze feature importance using SHAP values.
Conclusion
This project demonstrates the application of machine learning models to predict property prices in NYC. The analysis highlighted the importance of features like Gross Square Feet and Land Square Feet in predictions. XGBoost showed a slight advantage over Linear Regression, providing a more nuanced understanding of the factors driving property prices.

Contributing
Contributions to this project are welcome. Please fork the repository and submit a pull request with your improvements.

License
Distributed under the MIT License. See LICENSE for more information.
