# README for Leveraged Trading Strategies

## Overview

This project involves developing algorithmic trading strategies to generate profits from trading the SPTL ETF, which tracks long-term Treasury bonds. The strategies are based on historical data from 2014 to 2019, with an emphasis on risk management and performance optimization. This project explores different trading strategies including trend following, momentum, and mean-reverting, leveraging Python for data processing and analysis.

## Project Structure

Report.pdf: Detailed report on the methodology, strategies, results, and analysis.
Code.ipynb: Jupyter notebook containing the Python code for data collection, processing, strategy implementation, and analysis.

## Requirements

Python 3.x
Jupyter Notebook
Pandas
Matplotlib
yfinance

## Setup and Usage

Clone the Repository:
git clone <repository_url>
cd <repository_directory>

## Install Dependencies:
Ensure you have the required Python libraries installed. You can use pip to install them:
pip install pandas matplotlib yfinance

## Run the Jupyter Notebook:
Open the Jupyter notebook to explore the data processing, strategy implementation, and analysis:
jupyter notebook Code.ipynb

## Methodology

Data Collection and Preparation
SPTL Data: Extracted from Yahoo Finance using the yfinance library.
Effective Fed Funds Rate (EFFR) Data: Retrieved from the New York Federal Reserve website.
Data Merging: Both datasets were cleaned and merged based on dates, with the daily risk-free rate calculated.

## Trading Strategies

# Trend Following Strategy
Captures gains by looking at asset momentum in specific directions (up, down, or sideways).
Positions are modified based on the comparison of current and previous day's prices.

# Momentum Trading Strategy
Utilizes the momentum of price movements to make trading decisions.
Positions are adjusted based on positive or negative excess returns.

# Mean-Reverting Strategy
Assumes that prices will revert to their mean values over time.
Trades are made based on the comparison of current prices with a 30-day rolling average.

# Performance Metrics
Sharpe Ratio: Measures risk-adjusted returns.
Sortino Ratio: Focuses on downside risk-adjusted returns.
Maximum Drawdown: Assesses the worst-case scenario for losses.
Calmar Ratio: Relates annualized return to maximum drawdown.

## Results
Detailed analysis of the performance of each strategy, including cumulative profit and loss, turnover, and risk metrics.
Evaluation of the impact of increased funding costs on strategy performance.
Comparative analysis of the strategies against a buy-and-hold approach.

## Conclusion
This project demonstrates the implementation and evaluation of different algorithmic trading strategies using historical data. The analysis provides insights into the effectiveness and risks associated with each strategy, offering valuable information for making informed trading decisions.
