# Trading-using-ML
# Trading using Machine Learning

This project implements a trading strategy using machine learning techniques. The strategy involves downloading stock data, calculating technical indicators, clustering stocks, and optimizing a portfolio based on historical returns.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Trading Strategy](#trading-strategy)
- [Features](#features)
- [Contributing](#contributing)


## Overview

The goal of this project is to create a trading strategy that leverages machine learning to identify and exploit patterns in stock market data. The strategy includes:

1. Downloading historical stock data for S&P 500 companies.
2. Calculating various technical indicators.
3. Clustering stocks based on their features.
4. Optimizing a portfolio using historical returns.
5. Comparing the strategy's performance to a benchmark.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/trading-ml.git
    cd trading-ml
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Run the main script:
    ```sh
    python main.py
    ```

2. The script will download stock data, calculate technical indicators, cluster stocks, and optimize a portfolio. The results will be visualized and compared to a benchmark.

## Trading Strategy

### Data Downloading

The script downloads historical stock data for S&P 500 companies using the `yfinance` library. The data includes daily prices and volumes.

### Technical Indicators

Several technical indicators are calculated for each stock, including:

- **Garman-Klass Volatility**: A measure of stock volatility.
- **Relative Strength Index (RSI)**: A momentum oscillator that measures the speed and change of price movements.
- **Bollinger Bands**: A volatility indicator that consists of a middle band (simple moving average) and two outer bands (standard deviations).
- **Average True Range (ATR)**: A measure of volatility.
- **Moving Average Convergence Divergence (MACD)**: A trend-following momentum indicator.
- **Dollar Volume**: The product of adjusted close price and volume.

### Clustering

The stocks are clustered into groups using the K-Means clustering algorithm based on their calculated features. This helps in identifying similar stocks and diversifying the portfolio.

### Portfolio Optimization

The portfolio is optimized using the Efficient Frontier method from the `pypfopt` library. The optimization aims to maximize the Sharpe ratio, which is a measure of risk-adjusted return.

### Visualization

The strategy's performance is visualized and compared to a benchmark. The cumulative returns of the strategy and the benchmark are plotted over time.

## Features

- **Data Downloading**: Downloads S&P 500 stock data using `yfinance`.
- **Technical Indicators**: Calculates various technical indicators such as RSI, Bollinger Bands, ATR, and MACD.
- **Clustering**: Uses K-Means clustering to group similar assets.
- **Portfolio Optimization**: Optimizes the portfolio using the Efficient Frontier method.
- **Visualization**: Visualizes the portfolio returns and compares them to a benchmark.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.


