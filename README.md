# Bitcoin Price Prediction Using LSTM and Technical Indicators

This repository contains a model for predicting Bitcoin prices using Long Short-Term Memory (LSTM) neural networks and several technical indicators as input features. The model leverages historical Bitcoin price data and applies technical analysis to forecast future price movements.

## Project Overview

The goal of this project is to predict Bitcoin's future price by utilizing a machine learning approach, specifically LSTM, which is well-suited for time series forecasting. The model is trained on historical Bitcoin price data, combined with technical indicators like Moving Averages, Relative Strength Index (RSI), and Bollinger Bands to enhance predictive accuracy.

## Features

- **LSTM Model:** LSTM neural networks are effective for sequential data and time series prediction, helping to capture long-term dependencies.
- **Technical Indicators:** Various technical indicators are used as input features:
  - Exponential Moving Average (EMA): fast-medium-slow
  - Relative Strength Index (RSI)
  - Moving Average Convergence Divergence (MACD)

## Dataset

The dataset includes historical Bitcoin price data and technical indicators derived from price movements. It consists of daily OHLC (Open, High, Low, Close) prices and trading volume, alongside calculated technical indicators.

### Data Sources

- [Yahoo Finance](https://finance.yahoo.com/quote/BTC-USD/history/)

## Model Architecture

The architecture of the LSTM model used:
1. **Input Layer:** Includes price data and calculated technical indicators.
2. **LSTM Layers:** One layer of LSTMs is used to capture temporal patterns in the data.
3. **Dense Layer:** A fully connected layer is added to produce the final output.
4. **Output Layer:** Predicts future Bitcoin prices.

### Model Performance
The model performance is evaluated using several metrics:
- **Mean Absolute Error (MAE):** 0.01
- **Mean Squared Error (MSE):** 0.00
- **Root Mean Squared Error (RMSE):** 0.02
- **R-squared:** 0.99

These metrics indicate that the model achieves high accuracy in predicting Bitcoin prices.

## Requirements

To run the model, you will need the following dependencies:

- Python 3.11
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- pandas_ta (for technical indicators)

Install the dependencies using:

```bash
pip install -r requirements.txt
