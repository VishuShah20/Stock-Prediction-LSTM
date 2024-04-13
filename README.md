
# Microsoft Stock Forecasting with LSTMs

## Overview

This repository contains a project for forecasting Microsoft's stock prices using Long Short-Term Memory (LSTM) networks. The model is trained on historical stock data from Microsoft, spanning from 1986 to 2022, to predict future price movements. This approach utilizes the LSTM's ability to remember long sequences of data, which is ideal for time series forecasting like stock price movements.

## Use Case

This model is particularly useful for financial analysts and individual investors looking to get insights into potential future stock price movements of Microsoft. By understanding potential future prices, users can make more informed investment decisions.

## Features

- **Data Preprocessing**: Conversion of raw stock price data into a format suitable for LSTM training, including normalization and creating time-windowed sequences.
- **LSTM Model**: A neural network model that can capture the temporal dependencies of stock price movements.
- **Prediction**: The model outputs future stock price predictions based on the learned dependencies.
- **Visualization**: Graphical representation of the stock prices and predictions, providing clear visual insights into the model's performance.

## Getting Started

### Prerequisites

- Python 3.8+
- Libraries: TensorFlow, NumPy, Pandas, Matplotlib
- Data source: Historical stock prices from Yahoo Finance

## How It Works

1. Data Loading: The data is loaded into a Pandas DataFrame, showing the historical closing prices of Microsoft stocks.
2. Preprocessing: The data is preprocessed to fit the LSTM model; this includes scaling the data, creating training/validation/testing splits, and reshaping into sequences.
3. Model Building: An LSTM model is constructed using TensorFlow/Keras to predict future prices based on past data.
4. Training: The model is trained on the historical data, using a mean squared error loss function and an Adam optimizer.
5. Evaluation: The trained model is then used to predict stock prices, and the results are plotted against the actual prices to evaluate performance.
6. Prediction Visualization: Plots are generated to show how well the model's predictions match up with the actual stock prices over different intervals (training, validation, and testing).

### Installation

Clone this repository and install the required Python packages.

```bash
git clone https://github.com/your-username/microsoft-stock-forecasting.git
cd microsoft-stock-forecasting
pip install -r requirements.txt
