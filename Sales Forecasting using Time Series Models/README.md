# Superstore Sales Forecasting using Time Series:

## **Project Overview**

This project analyzes and forecasts daily sales data for a superstore using time series techniques. The goal is to uncover trends, seasonality, and patterns in the data, and to build predictive models for future sales. Methods include:

- **Exploratory Data Analysis (EDA)**
- **Statistical tests** (ADF, Shapiro-Wilk)
- **Time series decomposition**
- **SARIMA modeling**
- **Facebook Prophet**
- **XGBoost** for machine learning-based forecasting

## **Dataset**

The dataset contains daily sales data with the following key columns:

- **Date**: Transaction date.
- **Total**: Total sales amount (including tax).
- **Additional features**:
  - Branch
  - City
  - Customer type
  - Gender
  - Product line
  - Payment

## **Methodology**

### **Data Preprocessing**:
- Converted **Date** to datetime format.
- Extracted features like **Day**, **Month**, **Year**, and **Weekday**.

### **Exploratory Data Analysis (EDA)**:
- Analyzed **trends**, **seasonality**, and **outliers**.
- Visualized **daily sales** and **rolling averages**.

## **Visualizations**
- **Daily sales trends:**
<img src="https://github.com/user-attachments/assets/85c5e68d-7e8d-4892-b8b6-a9ff4d784d65" width="500">



- **Decomposition plot for Seasonality:**
<img src="https://github.com/user-attachments/assets/b0d034aa-84ad-4118-be37-5cb3b1f11076" width="500">



- **SARIMA forecast plot:** 
<img src="https://github.com/user-attachments/assets/48cc0017-2263-4bc9-9b88-61d3c14842ae" width="500">



**NOTE :** The intepretation of these graphs have been given in the code file.


### **Modeling**:
- **SARIMA**: Fitted using **auto_arima**.
- **Prophet**: Used for its ability to handle **seasonality**.
- **XGBoost**: Implemented with feature engineering (e.g., **lagged variables**).

### **Evaluation**:
- **Metrics**: **MAE**, **RMSE**, **MAPE**.
- Analyzed **residuals** for model adequacy.

## **Results**

### **Key Findings**:
- Daily sales show high variability with **weekly seasonality** (higher sales on Tuesdays and Fridays).
- No significant **outliers** detected.
- Data confirmed **stationary** via **ADF test**.

### **Model Performance**:

| Model   | MAE | RMSE | MAPE |
|---------|-----|------|------|
| SARIMA  | 959.09  | 1235.06    |  41.06%   |
| Prophet | 1248.30   | 1577.61    | 43.31%   | 
| XGBoost | 2.7768   | 5.0437    | 1.41%   |

### **Conclusion**:
This project analyzed and forecasted daily sales data for a superstore using time series techniques and machine learning. Key findings include:

- **Trends and Seasonality:** Daily sales exhibit high variability with weekly seasonality, peaking on Tuesdays and Fridays.

- **Model Performance:** XGBoost outperformed SARIMA and Prophet, achieving a MAPE of 1.41% compared to 41.06% (SARIMA) and 43.31% (Prophet). This improvement is attributed to XGBoost's ability to leverage rich feature engineering and capture non-linear relationships in the data.

- **Validation:** The results were validated to ensure no data leakage or overfitting, confirming the robustness of the XGBoost model.

This project demonstrates the power of combining time series analysis with machine learning for accurate sales forecasting. Future work could explore incorporating external factors (e.g., holidays, promotions) to further enhance model performance.
