# Machine Learning Stock Price Prediction
This project focuses on building, evaluating, and comparing machine learning models to predict the daily stock price for a given stock using historical stock data. It includes feature engineering, baseline regressors, and advanced models like KNN Regressor and Linear Regression.
## Overview
The predictions are evaluated using metrics like Mean Squared Error (MSE), Root Mean Squared Error (RMSE), R², and Mean Absolute Percentage Error (MAPE). Additionally, error plots are generated to visualize model performance.
## Dataset Features
The dataset contains the following columns for each stock:

CODE: Unique identifier for the stock.

NAME: Name of the stock.

12m Low / 12m High: Lowest and highest price over the last 12 months.

Day Low / Day High: Lowest and highest price during the current day.

Day Price: Closing price for the current day.

Previous: Previous day's closing price.

Change / Change%: Absolute and percentage change from the previous day.

Volume: Number of shares traded during the day.

Adjusted: Adjusted price after accounting for splits/dividends.

## Features Used
For predicting the Day Price, the following features are considered:

Day Low - Gives the upper range for the prediction

Day High - Gives the lower range for the prediction

Previous - Gives something like a starting point to avoid over shooting a prediction

## Models Implemented

### Baseline Regressors:

Constant (0).

Mean.

Median.

### KNN Regressor:

Hyperparameter tuning using GridSearchCV to find the best parameters for neighbors, weights, and distance metrics.

### Linear Regression:

A standard regression model to establish a benchmark for comparison

