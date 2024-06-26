## Table of Contents

- [Problem Statement](#ProblemStatement)
- [Solution](#solution)
- [Data Description](#data-description)
- [Tasks](#Tasks)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Feature Importance](#feature-importance)
- [Model Evaluation](#model-evaluation)
- [Usage](#usage)
- [Conclusion](#conclusion)


## Problem Statement

In Banking industry, loan applications are generally approved after a thorough background check of the customer's repayment capabilities. Credit Score plays a significant role in identifying customer's financial behavior (specifically default). However, people belonging to rural India don't have credit score and it is difficult to do a direct assessment. 

## solution

This project aims to predict the maximum loan amount that can be granted to rural customers who lack traditional credit scores. The prediction model uses various personal, financial, and house-related details of the customers to determine their repayment capabilities.

## Data Description

The dataset `trainingData.csv` contains the following information:
- `Id`: Primary Key
- Personal Details: `city`, `age`, `sex`, `social_class`
- Financial Details: `primary_business`, `secondary_business`, `annual_income`, `monthly_expenses`, `old_dependents`, `young_dependents`
- House Details: `home_ownership`, `type_of_house`, `occupants_count`, `house_area`, `sanitary_availability`, `water_availability`
- Loan Details: `loan_purpose`, `loan_tenure`, `loan_installments`, `loan_amount`

## Tasks

•	Do a descriptive analysis of all the variables. 

•	There is a new customer who needs a loan. Which models will be best suited to predict the loan_amount that can be granted to the customer?

•	Build a model to predict the maximum loan_amount that can be granted to the customer. Which all variables are good predictors?

•	Is loan_purpose a significant predictor? The business has insisted on using loan_purpose as a predictor. If it is not already a significant contributor, can we still modify the model to include it?

•	How will you measure the fitness of the model? Which metrics (accuracy, recall, etc.) are most relevant?



## Data Preprocessing

Data preprocessing steps include:
- Handling missing values
- Encoding categorical variables

## Model Building

We explored several regression models, including:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor (SVR)
- 
We selected Random Forest due to their performance and ability to handle non-linear relationships.

## Feature Importance

Feature importance analysis using models like Random Forest and XGBoost highlighted key predictors such as:
- Annual Income
- Monthly Expenses
- Primary Business Type
- Home Ownership and House Details

## Model Evaluation

We used the following metrics to evaluate model performance:
- Mean Squared Error (MSE)
- R-squared (R²)

## Usage

1. **Preprocess the New Customer Data**: Ensure the new customer data is formatted and encoded similarly to the training data.

2. **Predict Loan Amount**: Use the trained model to predict the loan amount.

