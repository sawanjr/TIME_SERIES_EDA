# Tesla Stock Time Series Analysis

This README file provides an overview of the exploratory data analysis (EDA) performed on the Tesla (TSLA) stock price time series data. The analysis is conducted using Python and various data manipulation and visualization libraries, including pandas and Matplotlib. The primary goal of this analysis is to gain insights into the historical stock price behavior of Tesla.

## Data Source
The data used for this analysis is sourced from a CSV file named "TSLA.csv." It contains historical Tesla stock price data with the following columns:
- Date: The date of the stock price data (converted to datetime).
- Open: The opening price of Tesla stock.
- High: The highest price of Tesla stock during the trading day.
- Low: The lowest price of Tesla stock during the trading day.
- Close: The closing price of Tesla stock.
- Adj Close: The adjusted closing price of Tesla stock.
- Volume: The trading volume of Tesla stock.

## Data Preprocessing
The following preprocessing steps were applied to the dataset:
- The "Date" column was converted to a datetime data type.
- The "Date" column was set as the index of the DataFrame.
- The "Date" column was dropped from the DataFrame.

## Exploratory Data Analysis (EDA)
The EDA included the following analyses and visualizations:

### 1. Stock Price Plot
A line plot of the "Open" column was created to visualize the daily opening prices of Tesla stock.

### 2. Stock Price Plot with Date Range
A line plot of the "Open" column was created with date range limits set from "2013-10-01" to "2020-12-01" to focus on a specific time period.

### 3. Date Index
An examination of the date index was conducted to understand the date range and frequency of the time series data.

### 4. Selecting Specific Rows by Indexing
Specific rows of the data were selected using date-based indexing, showing the open, high, low, close, adjusted close, and volume values for a specific date range.

### 5. Resampling
The concept of resampling was explained, including common resampling rules (e.g., 'A' for annual, 'Q' for quarterly, 'M' for monthly, etc.). Examples of resampling were provided, such as finding the maximum "Open" value within each calendar year and month.

### 6. Rolling
The rolling function was introduced, which is used to calculate rolling statistics (e.g., moving averages) for a time series. An example of a 5-day rolling mean of the "Open" column was demonstrated.

### 7. Rolling Mean Comparison
A comparison plot between the original "Open" column and a 30-day rolling mean of the "Open" column was created to visualize the smoothing effect of rolling statistics.

## Conclusion
This EDA provides a comprehensive overview of the Tesla stock price time series data, including basic data preprocessing, visualization of stock price trends, and exploration of resampling and rolling techniques. Further analysis and modeling can be performed based on these initial insights.

Data Overview:

The dataset contains 2,416 entries.
It includes columns such as Date, Open, High, Low, Close, Adjusted Close, and Volume.
The Date column has been converted to the datetime format.
Data Visualization:

The initial visualizations show the trends in the "Open" stock prices over time.
The plot with specific date limits (October 2013 to December 2020) provides a closer look at a specific time period.
Resampling techniques are applied to aggregate and analyze data at different frequencies, such as yearly, quarterly, and monthly.
Resampling Insights:

Yearly resampling was used to find the maximum "Open" price for each year. This can help identify annual trends and performance.
Quarterly resampling was applied to sum the values within each quarter. It provides insights into quarterly performance.
Monthly resampling was used to calculate the maximum "Open" price at the end of each month.
Rolling Mean Analysis:

Rolling mean calculations were performed to create a 30-day moving average of the "Open" prices. This smooths out short-term fluctuations in the data.
The rolling mean was visualized alongside the original "Open" prices to observe trends over a longer time horizon.
Business Days Resampling:

A "Business Year End" (BA) resampling technique was applied to consider business days and exclude weekends and holidays. This can be crucial for financial and business data analysis.
Data Visualization and Interpretation:

Line and kernel density plots were used to visualize the 30-day rolling mean of the "Open" prices. The rolling mean produces smoother trends, making it easier to identify long-term patterns.
Further Analysis:

Further analysis and modeling can be conducted on this dataset, such as predicting future stock prices or exploring correlations with other financial indicators.
