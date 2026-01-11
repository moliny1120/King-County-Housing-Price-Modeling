# King County Housing Price Modeling

## Overview
This project focuses on statistical modeling and inference for housing prices in King County, Washington.  
I developed multiple regression models to examine the relationships between housing prices and housing characteristics.

The goal of this project is to construct interpretable predictive models while carefully validating model assumptions and addressing common issues such as heteroskedasticity, non-normality, and multicollinearity.

## Data
- Dataset: King County housing sales data
- Observations: Residential housing transactions
- Response variable: Housing sale price
- Predictors include housing characteristics such as square footage, location, age, and other relevant attributes such as proximity to water.

## Methods
The modeling process includes the following steps:

- **Multiple Linear Regression (OLS)**
- **Regression diagnostics**
  - Linearity checks
  - Normality assessment (Q–Q plots)
  - Constant variance testing (Breusch–Pagan test)
  - Multicollinearity diagnostics (VIF)
- **Outlier and influence detection**
  - Mean shift tests
- **Transformations**
  - Box–Cox transformation to improve normality and variance stability
- **Weighted Least Squares (WLS)**
  - Addressed heteroskedasticity in the error structure
- **Variable selection**
  - LASSO regularization
  - Leaps-and-bounds subset selection
- **Model comparison and selection**
  - AIC
  - BIC
  - Adjusted R-squared
  - Mallows' Cp

## Results
The final selected model achieved improved predictive performance and better adherence to regression assumptions compared to the baseline OLS model.  

## Tools
- **Programming Language:** R
- **Statistical Libraries:** MASS, car, leaps, glmnet
- **Visualization:** ggplot2
- **Reproducibility:** R Markdown

## Repository Structure
```text
king-county-housing-price-modeling/
├── data/
│   └── README.md
├── scripts/
│   ├── data_cleaning.R
│   ├── modeling_ols.R
│   ├── diagnostics.R
│   └── variable_selection.R
├── figures/
├── README.md
└── .gitignore

