# 🌿 AI-Based Building Energy Consumption & Carbon Footprint Predictor

An end-to-end Machine Learning pipeline to predict building energy consumption (kWh) and calculate corresponding carbon footprint ($kg CO_2$) based on structural, operational, and environmental parameters.

## 📌 Project Overview
- **Domain:** Energy Efficiency & ESG / Sustainability Analytics
- **Task:** Regression & Feature Engineering
- **Environment:** Python, Google Colab

---

## 📐 Mathematical Framework & Methodology

### 1. Feature Engineering & Multi-collinearity (VIF)
To prevent multicollinearity, Variance Inflation Factor (VIF) was calculated across all continuous variables:
$$\text{VIF}_i = \frac{1}{1 - R_i^2}$$
*All features satisfied $VIF < 10$, confirming model stability.*

### 2. Carbon Footprint Equation
$$\text{Carbon Footprint } (kg\,CO_2) = \text{Predicted Energy Consumption } (kWh) \times 0.475$$

---

## 📊 Model Performance Benchmark

| Model | $R^2$ Score | RMSE | MAE |
|---|---|---|---|
| **Linear Regression** | **1.0000** | **0.0142** | **0.0122** |
| **Ridge Regression (L2)** | 0.9999 | 1.2961 | 1.1384 |
| **Random Forest** | 0.9792 | 119.5154 | 94.2362 |

---

## 🛠️ Tech Stack
`Python` `Pandas` `NumPy` `Scikit-Learn` `Statsmodels` `Matplotlib`
