## Project Overview

This project develops a **dual modeling framework** to forecast NVIDIA stock returns using both:

- **ARIMA (statistical time series modeling)**
- **Decision Tree (machine learning regression)**

The objective is to compare how well each approach captures stock behavior and generates reliable predictions.

### Overall Workflow
EDA → Stationarity → Feature Engineering → Model Training → Diagnostics → Evaluation

---

## 1. ARIMA Time Series Model

This component implements a complete **ARIMA pipeline** to model time-dependent structure in stock returns.

### Workflow
EDA → Stationarity → Model Identification → Model Fitting → Diagnostics → Forecast Evaluation

- **Descriptive visualization**
- **Stationarity testing (ADF)**
- **Train–test split (80% / 20%)**
- **Model identification (ACF/PACF)**
- **ARIMA model fitting (ARIMA(p,d,q))**
- **Residual diagnostics (autocorrelation, normality)**
- **Forecast evaluation (MSE, MAE, RMSE)**

### Tools
- **Data**: yfinance  
- **Analysis**: pandas, numpy  
- **Modeling**: statsmodels, pmdarima  
- **Diagnostics**: statsmodels, scipy  
- **Evaluation**: scikit-learn  
- **Visualization**: matplotlib  

### Results

**Model:** ARIMA(1, 0, 1)  

**Residual diagnostics:**  
- Residuals approximately normally distributed  
- No significant autocorrelation  

**Performance:**  
- RMSE: 0.1326  
- MAE: 0.1086  
- MSE: 0.0176  

---

## 2. Machine Learning Model: Decision Tree

This component applies a **Decision Tree Regressor** to capture non-linear relationships using engineered features.

### Workflow
EDA → Feature Engineering → Model Training → Evaluation

- **Descriptive visualization**
- **Feature engineering (lag variables, rolling mean, momentum)**
- **Train–test split (80% / 20%)**
- **Decision Tree model fitting**
- **Prediction on test data**
- **Evaluation (MSE, MAE, RMSE)**

### Tools
- **Data**: yfinance  
- **Analysis**: pandas, numpy  
- **Modeling**: scikit-learn (DecisionTreeRegressor)  
- **Evaluation**: scikit-learn  
- **Visualization**: matplotlib  

### Results

**Model:** Decision Tree Regressor  

**Performance:**  
- RMSE: 0.0326  
- MAE: 0.0175  
- MSE: 0.0011  

---
