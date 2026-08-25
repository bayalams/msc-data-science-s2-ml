# Marketing Campaign Response Prediction

## Overview

This project predicts whether a customer is likely to respond positively to a marketing campaign. The portfolio version exposes the actual exploratory and modelling work rather than only a final summary.

Because campaign-response data are imbalanced, the modelling objective is not simply to maximize accuracy. The work focuses on **ROC-AUC, precision, recall, F1, probability thresholds and the business value of campaign decisions**.

## Notebook guide

| Notebook | What it shows |
|---|---|
| `01_data_understanding_and_eda.ipynb` | business framing, customer EDA and response-pattern analysis |
| `02_logistic_regression.ipynb` | normalized Logistic Regression, class weighting, tuning and threshold evaluation |
| `03_random_forest.ipynb` | tree-based classification, tuning and feature importance |
| `04_extra_trees.ipynb` | Extra Trees modelling and nonlinear feature analysis |
| `05_mlp_pca.ipynb` | neural-network classification with PCA and Optuna |
| `06_model_comparison_and_business_decision.ipynb` | cross-model synthesis, threshold selection and campaign economics |

## Techniques demonstrated

- customer and campaign exploratory analysis
- customer-level feature engineering and RFM-style features
- missing-value handling
- scaling, log transforms and categorical encoding
- class weighting
- Logistic Regression
- Random Forest and Extra Trees
- MLP and PCA
- GridSearchCV and Optuna
- ROC-AUC, precision, recall, F1 and log-loss
- decision-threshold optimisation using a campaign profit function

## Selected saved results

Completed experiments included:

- Extra Trees ROC-AUC: **0.904**
- Random Forest positive-class F1: **0.652**
- MLP + PCA threshold-tuned F1: **0.662**
- Normalized Logistic Regression positive-class recall: **0.800** at the default threshold

For the MLP + PCA experiment, a threshold of **0.26** produced approximately **61.0% precision**, **72.3% recall**, **0.662 F1**, and **€286 simulated campaign profit** under the assumptions used in the notebook.

## Why the project matters

The project connects predictive performance to the decision being supported. A high-accuracy classifier can still perform poorly on the minority class, while a tuned probability threshold can materially change campaign outcomes.

## Data

The dataset is intentionally not redistributed. See `data/README.md` for the expected local filenames.

## Portfolio note

The notebooks are curated from completed MSc coursework. Code and saved outputs originate from the original work; presentation, paths and explanatory text have been cleaned for portfolio use.
