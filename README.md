# Predictive-modelling-Project

**Objective**: This report aims to predict firm sales using linear regression and analyze car crash data to predict survival rates using logistic regression and linear discriminant analysis (LDA).

**Problem 1: Firm Sales Prediction**

1. **Data Description**:
   - Dataset: 759 firms with attributes like sales, capital, patents, R&D stock, employment, S&P 500 membership, Tobin's q, stock market value, and proportion of stock owned by institutions.
   - Missing Values: Tobin's q had 21 missing values, imputed with the mean.

2. **Analysis**:
   - Univariate: Sales, capital, patents, R&D stock, and employment are right-skewed.
   - Bivariate: Sales highly correlated with capital, R&D stock, and employment.

3. **Modeling**:
   - Data Split: 70% training, 30% testing.
   - Linear Regression:
     - R²: 0.936 on training, 0.893 on testing.
     - RMSE: 2164.49 (train), 2953.57 (test).
   - Important Predictors: Employment, capital, and patents.

4. **Insights**:
   - The model predicts sales accurately.
   - Key factors influencing sales are employment, capital, and patents.

**Problem 2: Car Crash Survival Prediction**

1. **Data Description**:
   - Dataset: Car crash data with 11,217 records including attributes like weight, age, airbag, seatbelt, frontal impact, and survival status.
   - Missing Values: InjSeverity had 77 missing values, imputed with modal values.

2. **Analysis**:
   - Univariate: Most cars weigh 0-5000 lbs, occupants are aged 20-40, and vehicle models are from 1990-2000.

3. **Modeling**:
   - Data Split: 70% training, 30% testing.
   - Logistic Regression:
     - Accuracy: 98% (train and test).
     - ROC_AUC: 0.991 (train and test).
   - LDA:
     - Accuracy: 96% (train and test).
     - ROC_AUC: 0.968 (train), 0.967 (test).

4. **Insights**:
   - Logistic regression outperforms LDA with higher accuracy and AUC.
   - Key predictors of survival are airbag deployment, seatbelt usage, and occupant age.

**Conclusion**: The linear regression model effectively predicts firm sales, identifying employment, capital, and patents as crucial factors. The logistic regression model accurately predicts car crash survival, highlighting the importance of airbags and seatbelts, providing valuable insights for investment and safety policy decisions.
