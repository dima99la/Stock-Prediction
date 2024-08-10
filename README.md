# Stock Price Prediction Using Machine Learning and LSTM

This project aims to predict the future stock prices of NVIDIA (NVDA) by leveraging historical stock data and various machine learning models, including Linear Regression, RandomForest, GradientBoosting, XGBoost, Support Vector Regression (SVR), and a Long Short-Term Memory (LSTM) neural network. The project explores and compares the effectiveness of different models in capturing the underlying patterns in stock price movements.

## Table of Contents

- [Project Overview](#project-overview)
- [Motivation](#motivation)
- [Methodology](#methodology)
- [Installation](#installation)
- [Usage](#usage)
- [Models Used](#models-used)
- [Results](#results)
- [Applications](#applications)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

Financial markets are complex and influenced by a wide range of factors, making accurate stock price prediction a challenging task. This project leverages machine learning techniques to model and predict stock prices, providing insights into the performance of different algorithms in this domain.

The project is designed to be modular and easily extendable, allowing users to experiment with different models, feature engineering techniques, and prediction horizons. By comparing traditional machine learning models with deep learning models like LSTM, the project demonstrates the strengths and limitations of each approach in time series forecasting.

## Motivation

The primary motivation behind this project is to explore the application of machine learning in financial markets, specifically in predicting stock prices. Given the complexity and volatility of stock markets, predicting future prices is not only a technical challenge but also has significant real-world implications for investors, traders, and financial analysts.

The project also aims to provide a learning resource for those interested in applying machine learning to finance, by showcasing how different models can be implemented and evaluated on real-world data.

## Methodology

### Data Collection
The project uses historical stock price data for NVIDIA (NVDA), obtained from Yahoo Finance. The data includes daily stock prices from January 1, 2023, onwards, along with additional features such as moving averages, RSI (Relative Strength Index), Bollinger Bands, MACD (Moving Average Convergence Divergence), and trading volume.

### Feature Engineering
Several technical indicators are calculated from the raw stock price data to serve as features for the machine learning models. These indicators are commonly used by traders to identify trends, momentum, and potential reversal points in the market.

### Model Selection
The project implements and compares multiple machine learning models:

- **RandomForestRegressor:** An ensemble method that uses multiple decision trees to improve prediction accuracy.
- **GradientBoostingRegressor:** A sequential ensemble method that builds models iteratively to correct errors from previous models.
- **XGBoost:** An optimized version of gradient boosting that is known for its speed and performance.
- **SVR (Support Vector Regression):** A model that finds the hyperplane that best fits the data, suitable for non-linear relationships.
- **LSTM (Long Short-Term Memory):** A type of recurrent neural network (RNN) that is well-suited for time series forecasting, as it can capture long-term dependencies in the data.

### Model Evaluation
Each model is trained on the historical data and evaluated using metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE). The models are then compared to determine which provides the most accurate predictions for the given stock.

### Visualization
The predicted stock prices are visualized alongside the actual prices using Plotly, an interactive graphing library. This allows for a clear comparison of the model's predictions against real market data.
