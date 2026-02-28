# Macroeconomic-driven-beta-forecasting-Brazil
# Conditional Beta Forecasting for Brazilian Equities

## Project Overview

This project evaluates whether machine learning models can improve the out-of-sample forecasting of time-varying CAPM betas for Brazilian equities.

Betas are estimated using rolling 12-month windows based on the classical CAPM definition:

beta_i,t = Cov(R_i,t , R_m,t) / Var(R_m,t)

The objective is purely predictive: to determine whether macroeconomic and market variables contain incremental forecasting information relative to a naïve benchmark.

---

## Research Question

Can machine learning models outperform a persistence benchmark in forecasting dynamic CAPM betas for Brazilian stocks under strict time-series validation?

---

## Methodology

### 1. Data

- Monthly macroeconomic and financial variables
- Rolling 12-month CAPM betas as dependent variables
- Multiple Brazilian equities

All data is treated as time series.

---

### 2. Forecasting Framework

To avoid look-ahead bias and data leakage, the project implements:

- Expanding window time-series cross-validation
- TimeSeriesSplit validation
- Strict separation between training and testing periods

No random shuffling is used.

---

### 3. Benchmark

The benchmark model is a persistence model:

Beta_t = Beta_{t-1}

Model performance is evaluated relative to this benchmark.

---

### 4. Models Implemented

- Linear Regression
- Random Forest
- XGBoost

All models are evaluated under identical time-series validation schemes.

---

## Evaluation Metrics

- Mean Squared Error (MSE)
- Out-of-Sample R²:

R2_OOS = 1 - (MSE_model / MSE_benchmark)

This metric evaluates whether the model adds predictive value beyond persistence.

---

## Reproducibility

### Requirements

Install dependencies:
deled as a function of macroeconomic state variables (conditional CAPM).
