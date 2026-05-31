# synent-task7-timeseriesanalysis-Kinari-Thummar
Time series analysis on Stock Price dataset — trend analysis, seasonality detection and optional forecasting of future values | Synent Technologies Internship

# Apple Stock (AAPL) Time Series Analysis

## Problem Statement
Apple Inc. stock price data from 2010 to 2024 is analyzed to
identify trends, measure volatility, detect seasonal patterns
and forecast future price movements using statistical methods.

## Dataset
- **Source:** Yahoo Finance via yfinance library
- **Stock:** Apple Inc. (AAPL)
- **Period:** January 2010 — January 2024
- **Total Trading Days:** 3521
- **Features:** Date, Open, High, Low, Close, Adj Close, Volume

## Approach

### 1. Trend Analysis
- Closing price visualization
- 30, 90 and 200 Day Moving Averages

### 2. Volatility Analysis
- Daily Returns calculation
- Return distribution analysis
- 30 Day Rolling Volatility

### 3. Seasonality Detection
- Seasonal Decomposition (Trend, Seasonal, Residual)
- Monthly average price pattern
- Yearly average price trend

### 4. Stationarity Testing
- ADF Test — confirmed NON-STATIONARY (p-value: 0.9934)
- Applied differencing to make series stationary

### 5. Volume Analysis
- Price vs Volume relationship
- Inverse correlation between price growth and trading volume

### 6. Forecasting
- ARIMA (5,1,0) model
- 30 Day price forecast

## Key Insights
- Apple stock grew from **$5 in 2010 to $195 in 2024**
- **2023** recorded the highest yearly average price of ~$168
- **COVID-19 (2020)** caused the largest volatility spike of 6.0
- Daily returns are balanced around **mean of +0.11%**
- Clear **seasonal price peaks** in August-December tied to
  iPhone launches and holiday shopping season
- Trading volume **inversely correlates** with rising price —
  investors chose to hold as Apple became more valuable
- ARIMA forecasts **price stability around $190** for next 30 days

## Analysis Report
See [apple_stock_analysis_report.md](apple_store_stock_analysis_report.md)
for the complete analysis report with all insights.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Statsmodels
- yfinance
- Jupyter Notebook