# NJ Home Price Forecasting

A predictive analysis project to forecast home prices in New Jersey using R programming. This project applies data analysis and forecasting techniques to understand price trends.

## Project Overview

- **Objective**: To predict future housing prices in New Jersey using historical data and advanced forecasting models.
- **Tools**: R, R Markdown
- **Libraries Used**: Fpp, Fpp2, TTR, dplyr, ggplot2, forecast.

## Table of Contents
1. [Data Collection](#data-collection)
2. [Data Preprocessing](#data-preprocessing)
3. [Modeling](#modeling)
4. [Results](#results)
5. [Usage](#usage)
6. [Contributing](#contributing)

## Data Collection

Briefly describe the dataset used (source, time period, key columns). Mention if any data cleaning steps were necessary.

## Data Preprocessing

Explain any transformations, feature engineering, or cleaning steps performed.

## Modeling

Describe the models you explored, such as:
- **Baseline Model**: [e.g., Linear Regression]
- **Advanced Model**: [e.g., ARIMA, LSTM]
Mention any model evaluation metrics you used.

## Results

Model Performance Summary
Naive Forecast:

ME: 772.093, RMSE: 929.6161, MAE: 790.6977
MAPE: 0.2678, MASE: 0.0855, ACF1: 0.6471
This model exhibited the highest Mean Error (ME) and Root Mean Square Error (RMSE), indicating it was the least accurate among the models.
Simple Exponential Smoothing (SES):

ME: 754.5426, RMSE: 919.0724, MAE: 772.871
MAPE: 0.2618, MASE: 0.0836, ACF1: 0.6453
SES improved slightly over the naive forecast, showing a small reduction in RMSE and other error metrics.
Holt-Winters (HW) Additive Model:

ME: 82.1111, RMSE: 700.8931, MAE: 543.4792
MAPE: 0.1859, MASE: 0.0588, ACF1: 0.2658
The HW model produced the lowest error rates, indicating it was the most accurate in forecasting home prices.
Analysis & Conclusion
Best Forecast: Holt-Winters’ model, as it has the lowest error rates across all metrics, suggesting it captures the seasonality and trend effectively.
Forecast Trend: The time series analysis indicates an upward trend in home prices over the next 1–2 years.
Residual Analysis: The residuals in Holt-Winters appear random, with all ACF values within the confidence interval, affirming the model’s robustness in capturing data patterns.

## Usage

Instructions on running the code:
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/NJ_Home_Price_Forecasting.git
    ```
2. Open the `.Rmd` file in RStudio to view and execute the code.

## Contributing

Contributions are welcome! Please feel free to fork the project, create a branch, make your changes, and open a pull request.
