# PHASE-2-NEW-PROJECT
# INSIGHTS ON HOUSE PRICES

## 1. BUSINESS UNDERSTANDING.
The Business Understanding phase focuses on understanding the objectives and requirements of the project.Any good project starts with a deep understanding of the customer's needs.


### PROBLEM STATEMENT
This project seek to address the importannce of identifying the factors that significantly affect house prices.By conducting multiple regression, we can identify the relationship between different factors and house sales prices, taking into account the collective impact of multiple independent variables.

### OBJECTIVES

1. Conduct explanatory data analysis to gain insights on the relationships between different variables and target variable, assisting in selection of relevant variables for regression model.
2. Develop multiple regression model to predict house sale prices, considering the selected independent variables and their impact on the dependent variable.Validate the model assumptions, assess its goodness of fit and refine the model if necesssay.
3. Interpret the coefficients of the independent variables in the model to determine their individual impact on house prices, identifying the most influential factors driving thr house sales prices and their respective effects.
4. Evaluate and validate the performnance of the model.
5. Provide actionable insights and recommendations based on the analysis to assist real estate investors, and policymakers in making informed decisions regarding property investment, market trends, and economic planning.

### NOTEBOOK STRUCTURE
1. Reading the data.
2. Data Cleaning and Preprocessing.
3. Multiple Regression Modelling.
4. Model Evaluation and Undesrtanding.
5. Results Presentation and Conclusions.
6. Recommendations

## 2.IMPORTING PACKAGES AND LIBRARIES
# Importing packages for regresion analysis
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt 
%matplotlib inline
import warnings
warnings.filterwarnings("ignore")
from sklearn.model_selection import train_test_split 
from sklearn.linear_model import LinearRegression 
from sklearn.metrics import mean_squared_error, r2_score                     

## PROJECT SUMMARY
 Business Understanding
 Real estate agents can benefit from the regression analysis by understanding the factors that influence house prices. They can utilize the regression model to provide more accurate price estimates to their clients, identify key features to highlight in property listings, and make informed recommendations to buyers and sellers. We could also consider Homeowners and sellers who can use the regression model to estimate the potential value of their properties. By considering the influential features identified in the regression analysis, they can assess the impact of certain improvements or renovations on the property's price and make informed decisions regarding pricing and marketing strategies.

# Data Understanding
The dataset used in this project contains information about the factors affecting the housing prices including variables such as date, sqft_above, view and sqft_basement. Explanatory data analysis will be used to get a clear understanding of the dataset including the missing values, checking the data types, identifying outliers and also extracting relevant features for analysis. 

# Methodology
The methodology provides a structured approach to conduct the analysis using multiple regression modeling.It ensures appropriate handling of data, selection of relevant variables,model development, and validation to achieve accurate and reliable insights into the factors impacting house sale prices.

# Regression
Mean Squared Error (MSE): The MSE measures the average squared difference between the predicted and actual values. In this case, the MSE value is 39,411,843,010.30116. A lower MSE indicates better model performance, with smaller differences between predicted and actual values.

R-squared (R2) Score: The R2 score represents the proportion of the variance in the target variable that can be explained by the model. The R2 score ranges from 0 to 1, where 0 indicates that the model does not explain any of the variance and 1 indicates a perfect fit. In this case, the R2 score is 0.7011, indicating that approximately 70.11% of the variance in the target variable is explained by the model. A higher R2 score indicates a better fit.