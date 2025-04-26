# Yahoo Stock Price Prediction System

## Overview
The project implements an entire machine learning pipeline with the ability to forecast stock prices based on historical data pertaining to the market. The system incorporates feature engineering, dimensionality reduction, and several modeling approaches to predict the value of stocks in the future.

## Features

- **Data Processing**:
  - Time-series specific data cleaning
  - Chronological ordering and datetime handling
  - Normalization using MinMax scaling

- **Feature Engineering**:
  - Lag features (1, 2, 3, 5, 10-day intervals)
  - Rolling statistics (5/10-day means and standard deviations)
  - Temporal features (month, day, weekday extraction)
  - Correlation-based feature selection
  - PCA for dimensionality reduction

- **Modeling**:
  - LSTM neural networks for sequence prediction
  - SVM with hyperparameter tuning via GridSearchCV
  - Random Forest regression


## Usage Instructions

### Prerequisites
- Python 3.7+ environment

### Getting Started
1. **Prepare your data**:
   - Place your stock data file (`yahoo_stock.csv`) in the project root directory
   - Ensure the CSV contains required columns: Date, Open, High, Low, Close, etc.

2. **Launch the notebook**:
   ```bash
   jupyter notebook stock_prediction.ipynb
   ```

3. **Execute the notebook:**
    - Run cells in sequence usually from top to bottom
    - Wait for the execution of a cell before proceeding