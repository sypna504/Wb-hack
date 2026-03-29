# Wb-hack

Time series hackathon project focused on forecasting demand-like target values from route-based historical data.  
The repository contains exploratory data analysis, feature engineering experiments, a custom evaluation metric, and an initial forecasting pipeline built in Jupyter Notebook.

> **Project status:** this is **not the final version** of the solution.  
> The repository currently contains a working draft with experiments, intermediate analysis, and an initial modeling setup.

## Overview

The project is based on historical time series data with route identifiers, timestamps, multiple status features, and the target variable `target_1h`.  
The main goal is to explore patterns in the data, engineer useful time-based features, and build a baseline forecasting approach for future predictions.

## Features

- **EDA** — exploratory analysis of the training dataset
- **Feature Engineering** — creation of calendar and lag-based features
- **Custom Metric** — implementation of `WAPE + Relative Bias`
- **Time Series Analysis** — route-level and time-based pattern inspection
- **Forecasting Baseline** — initial setup using `MLForecast` and `CatBoost`
- **Notebook Workflow** — all experiments and intermediate results are collected in a single Jupyter Notebook

## Tech Stack

- **Language:** Python
- **Environment:** Jupyter Notebook
- **Data Analysis:** NumPy, pandas
- **Visualization:** matplotlib
- **Forecasting:** utilsforecast, MLForecast
- **Modeling:** CatBoost
- **Data Format:** Parquet

## Repository Structure

```text
.
├── solution.ipynb              # Main notebook with EDA, features, metric, and modeling draft
├── train_solo_track.parquet    # Training dataset
└── test_solo_track.parquet     # Test dataset
