NYC Property Sales Price Prediction
Overview
This project focuses on predicting property sale prices in New York City using machine learning models like Linear Regression and XGBoost. The data comes from the NYC Citywide Rolling Calendar Sales dataset. The project involves cleaning the data, building models, and evaluating their performance.

Dataset
The dataset contains information about property sales, with features like:

Neighborhood
Building Class
Land Square Feet
Gross Square Feet
Year Built
Sale Price
Key Steps
1. Data Preprocessing
Clean the data by removing rows with missing values.
Convert text-based numbers (e.g., "1,000") to numeric format.
Use pipelines to process numerical and categorical data.
2. Data Visualization
Histogram: Shows the distribution of Sale Price.
Scatter Plot: Explores the relationship between Gross Square Feet and Sale Price.
3. Model Training
Linear Regression: Trained as a simple baseline model.
XGBoost: Trained to improve prediction accuracy.
4. Model Evaluation
MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
R² Score: Measures how well the model explains the variance in the data.
5. Feature Importance
Permutation Importance: Identified which features impact the model the most.
6. SHAP Analysis
Used SHAP (SHapley Additive exPlanations) to explain individual predictions and understand global feature importance.
Results
Linear Regression:

MAE: 1,220,872
RMSE: 7,550,325
R²: 0.07
XGBoost:

MAE: 1,112,774
RMSE: 7,552,393
R²: 0.07
XGBoost performed slightly better than Linear Regression.

Visualizations
Partial Dependence Plot (PDP): Shows how features like Gross Square Feet affect predictions.
SHAP Plots: Visualize feature importance and how individual predictions are made.
How to Run
Preprocess the dataset.
Train models (Linear Regression and XGBoost).
Evaluate the models using MAE, RMSE, and R².
Analyze feature importance using SHAP.
Requirements
Install the following libraries:

bash
Copy code
pip install pandas matplotlib scikit-learn xgboost shap pdpbox joblib
Conclusion
This project demonstrates how machine learning models can predict NYC property prices. XGBoost performed better than Linear Regression, and feature analysis revealed the importance of Gross Square Feet and Land Square Feet in predicting sale prices.

Feel free to explore and improve the project!
