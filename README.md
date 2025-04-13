# Finanical_stock_market_Analysis
# AAPL Stock Analysis (Daily, Weekly, Monthly)

This repository contains an analysis of Apple Inc. (AAPL) stock data, covering daily, weekly, and monthly timeframes. The analysis includes data loading, cleaning, feature engineering, and visualization.

## Dataset

The dataset used in this project is sourced from Yahoo Finance, and consists of three CSV files:

* `AAPL_daily_update.csv`: Contains daily stock data.
* `AAPL_weekly_update.csv`: Contains weekly aggregated stock data.
* `AAPL_Montly_updates.csv`: Contains monthly aggregated stock data.
## Libraries Used

* `pandas`: For data manipulation and analysis.
* `matplotlib.pyplot`: For basic data visualization.
* `seaborn`: For enhanced data visualization.
* `numpy`: For numerical computations.

## Analysis Steps

### 1. Data Loading and Inspection

* Imported necessary libraries.
* Loaded the daily, weekly, and monthly CSV files into separate Pandas DataFrames.
* Inspected the DataFrame structures using `info()`, `head()`, and `shape`.
* Checked for missing values using `isnull().sum()` and handled them appropriately (e.g., `dropna()`, `fillna()`).
* Converted the 'Date' column to datetime objects and set it as the index for each DataFrame.
* Verified the DateTime index using `type(df.index)`.

### 2. Data Cleaning and Feature Engineering

* Calculated daily, weekly, and monthly returns using `pct_change()`.
* Calculated moving averages (50-day, 200-day) using `rolling().mean()`.
* Calculated volatility (standard deviation of returns) using `rolling().std()`.
* Calculated exponential moving averages (EMA) using `ewm().mean()`.

### 3. Exploratory Data Analysis (EDA)

* Plotted the adjusted close price over time for each frequency (daily, weekly, monthly).
* Plotted the distribution of daily, weekly, and monthly returns using histograms and kernel density estimates (KDE).

## File Structure
