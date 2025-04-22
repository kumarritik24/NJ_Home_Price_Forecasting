# 🏠 NJ Home Price Forecasting using R

📈 This project predicts median housing prices in New Jersey using time series forecasting techniques in **R**. It applies classical and decomposition-based models to uncover patterns and predict future values in the housing market.

---

## 📁 Project Overview

- **Objective**: Forecast median home prices in New Jersey using historical trends
- **Tools**: R, RMarkdown
- **Libraries**: `fpp`, `fpp2`, `TTR`, `dplyr`, `ggplot2`, `forecast`

---

## 🗂️ Table of Contents

1. [Data Collection](#data-collection)
2. [Data Preprocessing](#data-preprocessing)
3. [Modeling](#modeling)
4. [Results](#results)
5. [Usage](#usage)
6. [Contributing](#contributing)

---

## 📦 Data Collection

- Source: Median listing prices dataset for all homes in NJ  
- Format: `.csv` file, time-series indexed  
- Columns include: Region name, Date, Median Price

---

## 🔧 Data Preprocessing

- Converted time columns to time-series format
- Handled missing values and removed noise
- Created visual exploratory plots (trends & seasonality)

---

## 🤖 Modeling Approach

<details>
<summary>📉 Models Implemented</summary>

- **Baseline Models**:  
  - Naive Forecast  
  - Moving Average  
  - Simple Exponential Smoothing (SES)

- **Advanced Model**:  
  - Holt-Winters Additive  
  - Decomposition Additive (Season-Trend)

</details>

---

## 📊 Results Summary

| Model                 | RMSE     | MAE     | MAPE    |
|----------------------|----------|---------|---------|
| Naive                | 772.625  | 703.041 | 700.607 |
| Simple Exp Smoothing | 745.526  | 693.019 | 772.871 |
| Holt-Winters Additive| 611.131  | 520.891 | 514.702 |

✅ **Holt-Winters Additive** gave the **lowest error rates**, indicating superior performance in capturing both seasonality and trend.

---

## 🧠 Key Insights

- 📈 Forecast shows **upward housing trend** in NJ over the next 2–3 years
- 🧪 Holt-Winters model best captured the trend + seasonality
- 📉 Residual diagnostics confirmed randomness → robust forecasting

---

## ⚙️ Usage

```bash
# Clone the repo
git clone https://github.com/kumarritik24/NJ_Home_Price_Forecasting.git

# Open the .Rmd file in RStudio to run the code and generate output
