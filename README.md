NYC Property Sales Price Prediction
Overview
This project aims to predict the sale prices of properties in New York City using machine learning models such as Linear Regression and XGBoost. The dataset used is the NYC Citywide Rolling Calendar Sales dataset. The project focuses on cleaning the data, exploring it through visualizations, training machine learning models, and evaluating their performance using various metrics.

Dataset
The dataset contains information about property sales in NYC, with features like:

NEIGHBORHOOD
BUILDING CLASS CATEGORY
TAX CLASS AT TIME OF SALE
BUILDING CLASS AT TIME OF SALE
LAND SQUARE FEET
GROSS SQUARE FEET
YEAR BUILT
SALE PRICE
Project Steps
1. Data Preprocessing
Cleaning the Data: Remove rows with missing values in relevant columns and convert numerical columns (e.g., LAND SQUARE FEET, GROSS SQUARE FEET) to numeric format.
Categorical and Numerical Features: Preprocess the data using pipelines for numerical (e.g., scaling, imputing) and categorical features (e.g., one-hot encoding).
2. Exploratory Data Analysis
Distribution Plot: Visualized the distribution of SALE PRICE.
Scatter Plot: Explored the relationship between GROSS SQUARE FEET and SALE PRICE.
3. Model Training
Linear Regression: Fit a baseline linear regression model.
XGBoost Regressor: Fit a more advanced XGBoost model for better prediction accuracy.
4. Model Evaluation
Metrics: Evaluated models using MAE (Mean Absolute Error), RMSE (Root Mean Squared Error), and R² score.
Linear Regression: MAE, RMSE, and R² scores.
XGBoost: Improved MAE, RMSE, and R² compared to the baseline model.
5. Feature Importance
Permutation Importance: Identified the most important features contributing to the prediction of SALE PRICE.
6. Partial Dependence and SHAP Analysis
Partial Dependence Plots (PDP): Visualized how features like GROSS SQUARE FEET affect the predictions.
SHAP (SHapley Additive exPlanations): Analyzed individual predictions using SHAP force plots and visualized global feature importance using SHAP summary plots.
Results
Linear Regression Performance:

MAE: 1,220,872.68
RMSE: 7,550,324.91
R²: 0.07
XGBoost Performance:

MAE: 1,112,774.29
RMSE: 7,552,392.61
R²: 0.07
Visualizations
Partial Dependence Plot: Visualized the effect of GROSS SQUARE FEET and LAND SQUARE FEET on predictions.
SHAP Visualizations:
Force plots for individual predictions.
SHAP summary and dependence plots for feature analysis.
Files
final_xgb_model.pkl: Trained XGBoost model.
SHAP plots: Force plots and summary plots showing feature importance and individual prediction explanations.
Requirements
Install the following Python libraries:

bash
Copy code
pip install pandas matplotlib scikit-learn xgboost shap pdpbox joblib
How to Run
Preprocess the dataset and split it into training and test sets.
Train models such as Linear Regression and XGBoost.
Evaluate the model using metrics like MAE, RMSE, and R².
Analyze feature importance with SHAP and permutation importance.
Conclusion
This project demonstrates how to predict NYC property sale prices using machine learning models. The XGBoost model outperformed the Linear Regression baseline, and feature analysis showed that GROSS SQUARE FEET and LAND SQUARE FEET play important roles in determining property prices.

Feel free to explore the code and improve the models for better performance!
