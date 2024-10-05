# Understanding Concept of Financial Engineering 

File : Analyzing pirice stocks and crypto \\ need to make a table 


## Stochastic Modeling - Callibrating Merton and Heston Model 
The [Notebook](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Calibrating_Metron_and_Heston_Model.ipynb)focuses on calibrating the Merton Model, which is used in finance to assess credit risk and value debt. This involves implementing the model's logic and utilizing financial data, likely depicted in the included images. The process includes mathematical calculations, statistical analysis, and data manipulation using Python libraries like IPython. Overall, the notebook aims to accurately adjust the Merton Model's parameters to align with real-world financial data, enhancing its predictive capabilities for credit risk and debt valuation.

## Calculating return of Stocks using Yfinance APO 
code : [Here](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Working_with_stocks_return.ipynb)

## COOKS Distance 
Cook's distance is a statistical measure used to identify influential data points in regression analysis. It quantifies how much the predicted values for all cases would change if a specific data point were removed from the analysis.

Code :[Here](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Understanding_Cooks_Distance_.ipynb)


## Shapiro Test 

The Shapiro-Wilk test is a statistical hypothesis test used to determine if a sample of data comes from a normally distributed population. It is one of the most powerful tests for normality.

Null hypothesis (H0): The data is normally distributed.

Alternative hypothesis (H1): The data is not normally distributed

P-value > significance level (e.g., 0.05): Fail to reject the null hypothesis. There is not enough evidence to suggest the data is not normally distributed.


P-value <= significance level (e.g., 0.05): Reject the null hypothesis. There is sufficient evidence to suggest the data is not normally distributed.

Code [here](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Shapiro_Test.ipynb)

## Black Scholes model 

The Black-Scholes model is a mathematical formula used to calculate the theoretical value of a European-style option. It was developed by Fischer Black, Myron Scholes, and Robert Merton in the early 1970s.


1.)Simulating Geometric Brownian Motion (GBM): The notebook generates and visualizes GBM paths, illustrating how stock prices might evolve. It also calculates and plots the distribution of returns.

2.)Black-Scholes Model: The notebook demonstrates how to price a European call option using the Black-Scholes formula.

3.)Option Greeks: It calculates and explains the significance of Delta, Gamma, Vega, Theta, and Rho, which measure the sensitivity of option prices to various factors.

4.)Log-Normal Property of Stock Prices: The notebook analyzes historical stock prices and compares them to log-normal distributions, highlighting a key assumption of the Black-Scholes model

code : [here](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Black_Sholes_.ipynb)

## Y finance API and portfolio building 
The [Code](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/yfinance_1.ipynb) in the notebook does the following:

**Imports necessary libraries**: Installs and imports yfinance, pandas, numpy, and matplotlib.pyplot.
**Fetches stock data**: Downloads historical data for McDonald's (MCD), Exxon Mobil (XOM), and Walmart (WMT) using yfinance.
**Calculates daily returns**: Calculates the daily percentage change in closing prices for each stock.
**Computes descriptive statistics:** Calculates and prints the mean, standard deviation, skewness, and kurtosis of daily returns for each stock individually.
**Calculates correlations and covariances:** Computes and prints the correlation and covariance between daily returns of different stock pairs.
**Constructs a portfolio**: Creates a portfolio with equal weights (approximately) for the three stocks.
**Calculates portfolio statistics**: Calculates and prints the average return, volatility, skewness, and kurtosis of the portfolio returns.
**Visualizes skewness and kurtosis**: Generates a bar chart comparing the skewness and kurtosis of the portfolio returns.

## Time series Analysis of Magnificent Seven 

[Colab notebook ](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Time_series_analysis_M7.ipynb) Colab notebook analyzes stock data for the "Magnificent 7" tech companies (AAPL, MSFT, GOOGL, AMZN, NVDA, TSLA, META). It downloads historical data from Yahoo Finance and performs the following:

1. Data Preprocessing:

Handles missing values and ensures no remaining NaNs in the adjusted close prices.
Standardizes the data using StandardScaler.
2. Residual Analysis:

Builds a Linear Regression model to predict NVDA stock prices based on other stocks.
Plots residuals and predicted values to assess model fit.
3. Feature Extraction:

Statistical Features: Extracts mean, standard deviation, skewness, kurtosis, autocorrelation, etc.
Time-Based Features: Calculates rolling statistics, autocorrelation with different lags, skewness, and kurtosis.
Frequency Domain Features: Computes power spectral density and extracts features like mean, standard deviation, and entropy in the frequency domain.
Shape-Based Features: Identifies peaks and valleys, calculates their number and differences.
Lagged Features: Creates lagged features for time series analysis.
Window-Based Features: Uses Dynamic Time Warping (DTW) to identify similar motifs between stock pairs.
4. Time Series Decomposition:

Performs trend and seasonal decomposition using seasonal_decompose.
5. Dimensionality Reduction:

Applies Principal Component Analysis (PCA) to reduce the dimensionality of the data.
The notebook provides a comprehensive analysis of the stock data using various techniques for feature extraction, time series analysis, and dimensionality reduction
