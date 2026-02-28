# Macroeconomic-driven-beta-forecasting-Brazil
Macroeconomic-driven forecasting of time-varying betas for Brazilian publicly traded companies using econometric and machine learning models.
Work in progress.

Project Overview

This project develops a macroeconomic-based framework to forecast time-varying systematic risk (beta) for Brazilian publicly traded companies.

The model estimates rolling CAPM betas and evaluates whether macroeconomic variables improve out-of-sample forecasting performance relative to historical beta benchmarks.

Multiple modeling approaches are compared:

Linear Regression

Support Vector Machines

Random Forest

XGBoost

Neural Networks (MLP)

Recurrent Neural Networks (LSTM)

The objective is to assess whether systematic risk can be predicted using macroeconomic information.

Methodology

The project follows a structured financial engineering framework:

Estimation of rolling CAPM betas using 12-month rolling windows.

Construction of macroeconomic predictor variables, including lagged transformations.

Seasonal decomposition for selected macro variables.

Forecasting of time-varying betas using:

Linear Regression

Support Vector Machines (SVR)

Random Forest

XGBoost

Multi-Layer Perceptron (MLP)

Recurrent Neural Networks (LSTM)

Time-series-based train/test split (chronological).

Out-of-sample performance evaluation.

Data Description

Monthly frequency data.

Brazilian publicly traded companies.

Macroeconomic variables including:

Interest rates

Inflation measures

GDP-related indicators

Exchange rates

Commodity prices (WTI)

Sample period: (Specify your actual period here)

Note: Proprietary data is not included in this repository.

Model Validation

Models are evaluated using:

R² (coefficient of determination)

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

Rolling out-of-sample forecasting

Cross-validation

Baseline Comparison

Forecast performance is compared against:

Historical rolling beta

Naïve benchmark models

Limitations

Potential multicollinearity among macro variables.

Non-stationarity issues may affect parameter stability.

Machine learning models may suffer from overfitting in small samples.

Forecasting a parameter (beta) introduces estimation noise.

Future Improvements

Incorporation of regularization techniques (Ridge/Lasso).

Formal stationarity and cointegration testing.

Time-series cross-validation (walk-forward validation).

Economic regime-switching modeling.

## Theoretical Background

Under the CAPM framework, beta is defined as:

beta_i,t = Cov(R_i,t , R_m,t) / Var(R_m,t)

This project evaluates whether beta can be modeled as a function of macroeconomic state variables (conditional CAPM).
