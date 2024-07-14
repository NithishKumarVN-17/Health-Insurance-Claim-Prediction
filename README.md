# Insurance Claim Prediction

## Problem Statement

The insurance industry faces a critical challenge in charging each customer an appropriate premium based on their risk profile. Accurate prediction of claim amounts significantly impacts an insurer's management decisions and financial statements. This project aims to develop a more accurate and automated way to predict the cost of claims in an insurance company.

Several factors influence the cost of claims, including health indicators like BMI, age, smoking status, and various health conditions. Insurance companies employ numerous techniques to analyze and predict health insurance costs. This project explores and implements data-driven approaches to enhance the accuracy of these predictions.

## Data Definition

The dataset used for this project contains the following features:

1. **age**: Age of the policyholder (Numeric)
2. **sex**: Gender of policyholder (Categorical)
3. **weight**: Weight of the policyholder (Numeric)
4. **bmi**: Body Mass Index, providing an understanding of body weights relative to height (kg/m^2) (Numeric)
5. **no_of_dependents**: Number of dependent persons on the policyholder (Numeric)
6. **smoker**: Indicates if the policyholder is a smoker or non-smoker (non-smoker=0; smoker=1) (Categorical)
7. **claim**: The amount claimed by the policyholder (Numeric) - This is the target variable
8. **bloodpressure**: Blood pressure reading of policyholder (Numeric)
9. **diabetes**: Indicates if the policyholder suffers from diabetes (non-diabetic=0; diabetic=1) (Categorical)
10. **regular_ex**: Indicates if the policyholder regularly exercises (no-exercise=0; exercise=1) (Categorical)
11. **job_title**: Job profile of the policyholder (Categorical)
12. **city**: The city in which the policyholder resides (Categorical)
13. **hereditary_diseases**: Indicates if the policyholder suffers from hereditary diseases (Categorical)

## Project Goals

1. Analyze the provided dataset to identify patterns and correlations between various factors and claim amounts.
2. Develop and compare multiple predictive models to accurately estimate insurance claim amounts.
3. Evaluate model performance using appropriate metrics such as R-squared, Mean Absolute Error (MAE), and Adjusted R-squared.
4. Provide insights into the most influential factors affecting insurance claim amounts.
5. Create a reliable and scalable prediction system that can be used by insurance companies to estimate claim amounts for new policyholders.

## Methodology

1. Data Preprocessing: Clean the dataset, handle missing values, and encode categorical variables.
2. Exploratory Data Analysis: Visualize relationships between variables and the target claim amount.
3. Feature Engineering: Create new features or transform existing ones to improve model performance.
4. Model Development: Implement and train multiple machine learning models, including:
   - Linear Regression
   - Decision Tree
   - Random Forest
   - K-Nearest Neighbors (KNN)
5. Model Evaluation: Compare models using metrics such as R-squared, MAE, and Adjusted R-squared on both training and test datasets.
6. Model Interpretation: Analyze feature importance and model coefficients to understand key factors influencing claim amounts.

## Results

Based on the provided results for health insurance claim prediction models, here's a concise conclusion:

The Random Forest model appears to be the best performing overall, with high R-squared values for both training (0.99) and test (0.96) sets, indicating strong predictive power and generalizability. It also shows relatively low Mean Absolute Error (MAE) values.

The Decision Tree model achieves perfect fit on the training data (R-squared = 1.0) but shows slight overfitting when compared to its test performance (R-squared = 0.94).

Linear Regression and KNN models demonstrate good performance, but not as strong as Random Forest.

In summary, the Random Forest model seems to offer the best balance of accuracy and generalization for this health insurance claim prediction task.
