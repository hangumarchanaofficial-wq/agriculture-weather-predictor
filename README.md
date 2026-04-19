# Hyperlocal Rainfall Prediction ML

This repository contains a notebook-based machine learning workflow for predicting rainfall from weather data.

## Project Structure

- `data/raw/weather_data.csv`: original dataset
- `data/processed/cleaned_weather_data.csv`: cleaned dataset generated during preprocessing
- `notebooks/01_data_cleaning.ipynb`: data cleaning and preprocessing
- `notebooks/02_eda.ipynb`: exploratory data analysis
- `notebooks/03_model_training.ipynb`: feature preparation, model training, evaluation, and model selection
- `notebooks/04_prediction.ipynb`: prediction workflow

## Workflow

1. Run `01_data_cleaning.ipynb` to prepare the processed dataset.
2. Run `02_eda.ipynb` to inspect distributions and relationships in the data.
3. Run `03_model_training.ipynb` to train and compare candidate models.
4. Run `04_prediction.ipynb` to generate predictions.

## Notes

- The repository is intentionally kept focused on notebooks and datasets.
- Outputs stored inside notebooks may reflect the last local execution state.
