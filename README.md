# Hyperlocal Rainfall Prediction ML

This project is a notebook-driven machine learning workflow for predicting whether rainfall will occur from weather observations. It covers data cleaning, exploratory analysis, feature preparation, model training, and prediction.

## What Is Included

- `data/raw/weather_data.csv`: original weather dataset
- `data/processed/cleaned_weather_data.csv`: cleaned dataset produced during preprocessing
- `notebooks/01_data_cleaning.ipynb`: load, clean, and prepare the dataset
- `notebooks/02_eda.ipynb`: explore the data with summary statistics and visual analysis
- `notebooks/03_model_training.ipynb`: build features, train candidate models, compare results, and save the final model
- `notebooks/04_prediction.ipynb`: generate predictions from the trained model

## Problem Statement

The goal is to use historical weather measurements to predict `rain_or_not`, a binary target indicating whether rain occurred. The notebook workflow treats this as a supervised classification task.

## Dataset Overview

The cleaned dataset contains weather features such as:

- average temperature
- humidity
- average wind speed
- cloud cover
- pressure
- date-derived features such as day, month, and day of week

The target column is `rain_or_not`, where `1` indicates rain and `0` indicates no rain.

## Workflow

1. Run `01_data_cleaning.ipynb` to convert the raw dataset into a cleaned, analysis-ready file.
2. Run `02_eda.ipynb` to inspect distributions, class balance, and relationships between variables.
3. Run `03_model_training.ipynb` to train and evaluate multiple classifiers and select the final model.
4. Run `04_prediction.ipynb` to use the trained model for inference.

## Model Training Notes

The training notebook compares a few baseline classifiers and evaluates them with accuracy and ROC AUC. In the current notebook run, logistic regression performed best on the test split by ROC AUC.

## How To Run

1. Open the repository in Jupyter Notebook or JupyterLab.
2. Run the notebooks in order from `01_data_cleaning.ipynb` through `04_prediction.ipynb`.
3. Make sure the notebook kernel points to the same Python environment that has the required libraries installed.

## Repository Scope

This repository is intentionally kept lightweight and notebook-focused. The source package and several generated project artifacts were removed so the repo stays centered on the data and analysis workflow.

## Notes

- Notebook outputs may reflect the last executed state.
- If you rerun the notebooks, the saved outputs in the `.ipynb` files will update.
