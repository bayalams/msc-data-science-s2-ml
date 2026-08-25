# MSc Machine Learning Portfolio

A curated selection of machine-learning projects completed as part of MSc coursework and refined for portfolio use.

The repository is organised so that a reviewer can see both the **finished story** and the **actual analytical work**. Each main project contains a README plus a short sequence of cleaned notebooks covering data understanding, modelling and evaluation.

## Projects

### 1. Bike Rental Demand Prediction

Regression and time-aware forecasting of daily bicycle-rental demand using environmental, calendar and historical-demand information.

**Highlights:** chronological validation, feature engineering, Ridge Regression, Random Forest, LightGBM, MLP, GridSearchCV, Optuna, residual analysis and feature importance.

### 2. Marketing Campaign Response Prediction

Binary classification of customer campaign response, with emphasis on class imbalance, threshold selection and business-oriented model evaluation.

**Highlights:** Logistic Regression, Random Forest, Extra Trees, MLP, PCA, ROC-AUC, precision/recall, F1, Optuna and campaign-profit threshold optimisation.

## Repository structure

```text
Projects/
├── Project_1_Bike_Rental_Demand/
│   ├── README.md
│   ├── 01_data_understanding_and_preparation.ipynb
│   ├── 02_ridge_regression_baseline.ipynb
│   ├── 03_random_forest.ipynb
│   ├── 04_lightgbm.ipynb
│   ├── 05_mlp_optuna.ipynb
│   └── 06_project_summary_and_model_comparison.ipynb
└── Project_2_Marketing_Response/
    ├── README.md
    ├── 01_data_understanding_and_eda.ipynb
    ├── 02_logistic_regression.ipynb
    ├── 03_random_forest.ipynb
    ├── 04_extra_trees.ipynb
    ├── 05_mlp_pca.ipynb
    └── 06_model_comparison_and_business_decision.ipynb
```

`Tests/` can be retained separately for additional experimental variants, but it is no longer required as evidence of the main work because the strongest completed notebooks now live with each project.

## Data

Datasets are not redistributed unless their licensing/ownership permits it. Each project includes a `data/README.md` explaining the expected local filenames.

## Portfolio approach

The original coursework briefs are not reproduced. The notebooks preserve the actual analysis and saved results while cleaning presentation, file paths and explanatory text for public review.
