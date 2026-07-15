# German Electricity Demand Forecasting

## Project Overview

This project investigates German electricity demand forecasting using statistical, machine learning, and deep learning models. The analysis uses the Open Power System Data (OPSD) dataset and compares the forecasting performance of Benchmark models, SARIMA, SARIMAX, Random Forest, and Long Short-Term Memory (LSTM). The objective is to identify the most suitable forecasting model by comparing forecasting accuracy, interpretability, and model complexity.
---

## Objectives

- Forecast weekly German electricity demand.
- Compare multiple forecasting approaches.
- Evaluate models using RMSE, MAE, and MAPE.
- Assess the impact of temperature as an external variable.
- Recommend the most suitable model for operational forecasting.

---

## Dataset

The analysis uses the **Open Power System Data (OPSD)** Time Series dataset.

- Country: Germany
- Frequency: Hourly (aggregated to weekly)
- Period: January 2015 – October 2020

Dataset available at: https://open-power-system-data.org/

---

## Project Workflow

1. Data Collection
2. Data Preprocessing
3. Exploratory Data Analysis
4. Stationarity Testing
5. Benchmark Forecasting
6. SARIMA Model
7. SARIMAX Model
8. Random Forest Model
9. LSTM Model
10. Model Evaluation and Comparison

---

## Models Implemented

- Mean Forecast
- Naive Forecast
- Seasonal Naïve Forecast
- Drift Forecast
- SARIMA
- SARIMAX
- Random Forest
- Long Short-Term Memory (LSTM)

---

## Evaluation Metrics

The forecasting models were evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)

---

## Results

The forecasting models were compared using RMSE, MAE, and MAPE.

| Model | RMSE | MAE | MAPE (%) |
|--------|-----:|-----:|---------:|
| LSTM | 1429.71 | 1102.55 | 2.09 |
| SARIMA | 2674.83 | 2134.80 | 4.03 |
| Random Forest | 2688.14 | 1981.35 | 3.82 |
| Seasonal Naive | 3006.76 | 2318.52 | 4.41 |
| SARIMAX | 3055.21 | 2266.90 | 4.36 |
| Mean | 4397.30 | 3788.83 | 6.97 |
| Naïve | 4459.11 | 3783.20 | 6.79 |
| Drift | 5117.96 | 4339.89 | 8.05 |


## Best Model

The LSTM model achieved the best forecasting performance with an RMSE of **1429.71**, MAE of **1102.55**, and MAPE of **2.09%**. It outperformed all benchmark, statistical, and machine learning models, making it the recommended model for this dataset.

### Key Findings

- **LSTM** achieved the best overall forecasting performance with the lowest RMSE, MAE, and MAPE.
- **SARIMA** was the strongest statistical model, providing a good balance between accuracy and interpretability.
- **Random Forest** produced competitive results using engineered features.
- **Seasonal Naive** was the best benchmark because of the strong yearly seasonality in the dataset.

---

## Repository Structure

```
German-Electricity-Demand-Forecasting/
│
├── data/
├── figures/
├── outputs/
├── notebooks/
├── report/
├── README.md
└── requirements.txt
```

---

## Repository Contents

### notebooks/

Contains the complete Notebook used for data preprocessing, exploratory analysis, model development, forecasting, and evaluation.

### figures/

Contains all figures generated during the analysis, including:

- Weekly Electricity Demand
- Seasonal Decomposition
- ACF Plot
- PACF Plot
- Benchmark Forecast
- SARIMA Forecast
- SARIMAX Forecast
- Random Forest Forecast
- LSTM Forecast

### outputs/
Contains the exported model comparison results

### report/

Contains the final project report submitted for the assignment.
---

## Requirements

- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn
- TensorFlow (Keras)

Install using:

```bash
pip install -r requirements.txt
```

---

## How to Run

1. Download the OPSD dataset.
2. Place the dataset in the `data` folder.
3. Open the Jupyter Notebook.
4. Run all notebook cells sequentially.
5. Generated figures and outputs will be saved in their respective folders.

---

