## Overview

An FMCG company faces major demand–supply imbalance across its nationwide warehouses. Some regions experience frequent stockouts while others hold excess inventory, leading to wastage and higher carrying costs.

This project builds a data-driven demand forecasting and distribution optimization system to align supply with regional demand patterns.

## Problem Statement

Inefficient demand–supply planning across warehouses results in lost sales, excess inventory, increased storage costs, and product wastage. The absence of a predictive allocation system prevents optimal distribution and regional demand visibility.

## Objective

Develop a predictive model to forecast regional product demand and recommend optimal shipment quantities to each warehouse for efficient supply chain planning.

## Approach

• Performed exploratory data analysis to identify regional demand trends, seasonality, and inventory gaps.

• Engineered time-series and regional features; handled missing values, outliers, and preprocessing for model readiness.

• Built and compared five regression models:
Linear Regression, Random Forest, Gradient Boosting, AdaBoost, and XGBoost.

• Performed hyperparameter tuning on three high-performing ensemble models (Random Forest, Gradient Boosting, XGBoost) using GridSearchCV.

• Evaluated models using RMSE, MAE, and R² metrics and selected the best-performing model based on prediction accuracy and business suitability.

## Skill set applied

Python, Pandas, NumPy, Scikit-learn, XGBoost, EDA, Feature Engineering, Demand Forecasting, Regression Modeling, Model Evaluation (RMSE, MAE, R²), Hyperparameter Tuning.

## Result

Tuned ensemble models were compared on the test dataset:

• Tuned XGBoost (Final Model)
RMSE: ~7.90K tons | MAE: ~6.20K tons | R²: ~0.533

• Tuned Gradient Boosting
RMSE: ~7.91K tons | R²: ~0.533

• Tuned Random Forest
RMSE: ~7.93K tons | R²: ~0.530

XGBoost produced the lowest prediction error and highest explained variance and was selected as the final model.

The model’s accuracy indicates shipment forecasts typically deviate by ~7.9K tons, with an average allocation difference of ~6.2K tons, while explaining over 53% of demand variation. This enables reliable demand forecasting, optimized inventory allocation, and reduced logistics inefficiencies across warehouse networks.
