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
| SARIMA  | X   | Y    | Z%   |
| Prophet | A   | B    | C%   |
| XGBoost | D   | E    | F%   |

## **Visualizations**
- Daily sales trends.
- 7-day rolling average.
- SARIMA and Prophet forecasts.
