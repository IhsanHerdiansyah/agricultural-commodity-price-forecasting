# Agricultural Commodity Price Forecasting

A personal machine learning project for forecasting agricultural commodity prices using **Prophet, LSTM, and a hybrid Prophet + LSTM approach**.

## Overview

This project explores and compares three time-series forecasting approaches:

* **Prophet** — captures trend and seasonality.
* **LSTM** — learns patterns from historical time-series data.
* **Prophet + LSTM** — combines Prophet's trend and seasonal components with LSTM for hybrid forecasting.

The workflow covers data preparation, preprocessing, feature engineering, model training, forecasting, and evaluation.

## Data Options

The notebook supports three data sources:

1. **CSV Upload**
   Users can upload their own time-series dataset in CSV format with:

   * `date` — date in `YYYY-MM-DD` or `YYYY/MM/DD` format
   * `price` — commodity price

2. **Google Drive**
   A CSV dataset can be loaded directly from Google Drive.

3. **Synthetic Data Generator**
   The notebook can generate synthetic weekly time-series data containing simulated:

   * Trend
   * Annual seasonality
   * Seasonal shocks
   * Random noise

For the current project demonstration, the **synthetic data generator** was used.

## Workflow

```text
Data Input
    ↓
Preprocessing
    ↓
Feature Engineering
    ↓
Prophet
    ↓
LSTM
    ↓
Prophet + LSTM
    ↓
Evaluation
```

## Model Comparison

| Model          | Purpose                         |
| -------------- | ------------------------------- |
| Prophet        | Trend & seasonality forecasting |
| LSTM           | Historical sequence learning    |
| Prophet + LSTM | Hybrid forecasting approach     |

## Evaluation

Model performance is evaluated using:

* **RMSE (Root Mean Squared Error)**
* **MAE (Mean Absolute Error)**

The notebook also provides **Actual vs Predicted** visualizations for each approach.

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Prophet
* TensorFlow / Keras
* LSTM
* Matplotlib
* Google Colab

## Project Structure

```text
agricultural-commodity-price-forecasting/
│
├── Agricultural_Commodity_Price_Forecasting.ipynb
└── README.md
```

## Notes

This project is intended as a hands-on exploration of **time-series forecasting and machine learning**, using synthetic data to provide a controlled environment for comparing different forecasting approaches.
