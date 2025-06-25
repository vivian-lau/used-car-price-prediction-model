# 🚗 Used Car Price Prediction
The goal of this analysis was to develop a machine learning model that accurately predicts the selling price of used cars based on key features such as year, mileage (odometer), car type and other specifications. This helps dealers make informed decisions on pricing, trade-in offers, and inventory stocking.

Dataset: 
This project analyzes a dataset of over 426,000 used cars to identify what factors affect a car’s resale value and to predict prices using various regression models. It is intended to help used car dealers fine-tune their inventory and pricing strategies.
The dataset was obtained from Kaggle and contains vehicle listings with features such as:

- price
- year
- odometer
- manufacturer
- model
- fuel
- title_status
- transmission
- type
- region
- state, etc.

## 📊 Objective

The goal of this project is to:

1. Explore and clean the data
2. Identify features that influence price
3. Train and evaluate regression models to predict car prices
4. Recommend pricing strategies for car dealerships


## 🧹 Data Cleaning

- Dropped columns with >30% missing data
- Dropped rows that are missing > 2% of data
  - Categorical: replaced with unknown 
- Filtered out extreme values:
  - Price < \$1,000 or > \$500,000
  - Odometer outliers


## 📈 Exploratory Analysis using correlation analysis and heatmap

- **Correlation**: Strong negative correlation between price and odometer/age
- **Vehicle types**: Trucks and SUVs tend to retain more value

## 🤖 Models Used

We tested the following models:

- Linear Regression
- Decision Tree
- Random Forest Regressor
- XGBoost

## Evaluation Metrics:
- R² Score
- MAE


## 🏆 Best Model

The best-performing model was Random Forest Regressor with an R² of 0.80 and a low MAE of 0.005, indicating strong predictive performance across various vehicle types and conditions.

Key Insights for Inventory Optimization

Mileage (Odometer) and Year are the most predictive features. Newer cars with lower mileage dictate higher prices. Vehicle Type Matters. Trucks and pickups show greater price variance and importance than sedans or hatchbacks. Focus pricing strategy around Year + Mileage + Vehicle Type.



