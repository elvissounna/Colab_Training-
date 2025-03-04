# QuantStatsAnalyzing-

This repository contains code for generating a comprehensive dataset to analyze portfolio performance and risk characteristics using historical market data. The code leverages Python libraries such as `pandas`, `numpy`, and `yfinance` to download market data, calculate returns, and create a detailed dataset with various performance metrics.

## Features

- **Market Data Download**: Fetches historical adjusted closing prices for a set of selected tickers.
- **Performance Metrics Calculation**: Computes daily returns, cumulative values, and individual asset data.
- **Portfolio Creation**: Constructs a hypothetical portfolio with custom weights and calculates portfolio returns and value.
- **Benchmark Comparison**: Generates a synthetic benchmark based on the SPY ETF and compares its performance with the portfolio.
- **Dataset Creation**: Produces a comprehensive dataset including portfolio returns, portfolio value, benchmark returns, benchmark value, and individual asset values and returns.
- **Data Saving**: Saves the generated datasets to CSV files for further analysis and visualization.

## Requirements

- Python 3.x
- pandas
- numpy
- yfinance

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/portfolio-performance-analysis.git
    cd portfolio-performance-analysis
    ```

2. Install the required Python libraries:
    ```sh
    pip install pandas numpy yfinance
    ```

## Usage

1. Run the `generate_portfolio_dataset()` function to download market data and generate the dataset:
    ```python
    import pandas as pd
    import numpy as np
    import yfinance as yf
    from datetime import datetime, timedelta

    # Your code here...

    # Generate the dataset
    dataset, asset_allocation, market_data = generate_portfolio_dataset()
    ```

2. The generated datasets will be saved as `portfolio_performance_dataset.csv` and `asset_prices_dataset.csv`.

## Output

The generated dataset includes the following columns:

- `portfolio_returns`: Daily percentage returns of the portfolio.
- `portfolio_value`: Cumulative value of the portfolio starting with $10,000.
- `benchmark_returns`: Daily returns of a synthetic benchmark (SPY).
- `benchmark_value`: Cumulative value of the benchmark starting with $10,000.
- `[ticker]_value`: Cumulative value of each individual asset starting with $10,000.
- `[ticker]_returns`: Daily percentage returns for each asset.


