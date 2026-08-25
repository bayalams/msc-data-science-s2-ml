# Bike Rental Demand Prediction

## Overview

This project predicts daily bicycle-rental demand from calendar, weather and historical-demand information. It is presented as a sequence of curated notebooks so that the analytical process—not only the final results—is visible.

A central modelling choice is **time-aware validation**: because the objective is to predict future demand, model development preserves chronological order rather than randomly mixing earlier and later observations.

## Notebook guide

| Notebook | What it shows |
|---|---|
| `01_data_understanding_and_preparation.ipynb` | EDA, data-quality checks, feature decisions and creation of the modelling dataset |
| `02_ridge_regression_baseline.ipynb` | regularized linear baseline, tuning and residual analysis |
| `03_random_forest.ipynb` | nonlinear tree model, validation and feature diagnostics |
| `04_lightgbm.ipynb` | gradient boosting, tuning and error analysis |
| `05_mlp_optuna.ipynb` | neural-network regression with Optuna tuning |
| `06_project_summary_and_model_comparison.ipynb` | concise synthesis and final modelling lessons |

## Techniques demonstrated

- exploratory analysis of demand, calendar and weather variables
- feature engineering and data preparation
- time-aware / expanding-window validation
- Ridge Regression
- Random Forest
- LightGBM
- Multi-Layer Perceptron
- GridSearchCV and Optuna
- R², RMSE and MAE
- residual and feature-importance analysis

## Selected saved results

The original experiments recorded a progression from weaker linear baselines to stronger tuned nonlinear models. A later MLP experiment recorded a test R² of approximately **0.528** with RMSE of about **1,288 rentals**. Performance varied materially between temporal folds, reinforcing the need for time-aware validation.

## Data

The dataset is intentionally not redistributed. See `data/README.md` for the expected local filenames.

## Portfolio note

The notebooks are curated from completed MSc coursework. Code and saved outputs originate from the original work; presentation, paths and explanatory text have been cleaned for portfolio use.
