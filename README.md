# Understanding Concept of Financial Engineering 

File : Analyzing pirice stocks and crypto \\ need to make a table 



## Stochastic Modeling - Callibrating Merton and Heston Model 
The [Notebook](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Calibrating_Metron_and_Heston_Model.ipynb) focuses on calibrating the Merton Model, which is used in finance to assess credit risk and value debt. This involves implementing the model's logic and utilizing financial data, likely depicted in the included images. The process includes mathematical calculations, statistical analysis, and data manipulation using Python libraries like IPython. Overall, the notebook aims to accurately adjust the Merton Model's parameters to align with real-world financial data, enhancing its predictive capabilities for credit risk and debt valuation.

## Bates (1996) model calibration full for Asian Put Option
The [Notebook](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Bates_1996_Asian_Put.ipynb) calibrates the Bates (1996) model to Asian put option prices using market data. It calibrates the Heston (1993) sub-model first, then the jump component, and finally the full model. It also implements pricing using Lewis (2001) and Carr-Madan FFT and compares results to the market prices.

## Option Pricing with CIR and BCC Models
[Notebook](https://github.com/ParthDave111/Quant-and-Finance-File/blob/main/Option_pricing_with_CIR_and_BCC.ipynb), broken down by modules 1 to 4:

Module 1: Introduction and Setup

This module likely imports necessary libraries such as NumPy and SciPy.
It probably defines important variables and parameters like initial interest rates (r_0), volatility (sigma_r), and other financial constants.
The focus here is setting the stage for financial modeling.
Module 2: Cox-Ingersoll-Ross (CIR) Model

Introduces the CIR model for interest rate dynamics.
Defines a function CIR_forward_rate to calculate forward interest rates based on CIR model parameters.
Includes a function CIR_error_function that likely helps in calibrating the CIR model by finding the optimal parameters that minimize the difference between model-predicted and observed interest rates.
Module 3: Black-Cox (BCC) Option Pricing

Likely introduces the Black-Cox (BCC) model or Black '96 (B96) framework for option pricing.
The most important function here would be BCC_call_value which calculates the value of a European call option using this framework, taking inputs like the initial stock price (S_0), strike price (K), time to maturity (T), risk-free rate, and other parameters related to the model.
Module 4: Put-Call Parity and Calculation

This module applies the put-call parity relationship to calculate the price of a European put option.
It uses the previously calculated call option value (from BCC_call_value) and other parameters to determine the put option value.
The end goal is likely to output or display this calculated put option value.
Overall:

The notebook likely aims to illustrate a workflow in financial modeling, starting from setting up the environment, modeling interest rates (CIR), pricing a call option (BCC/B96), and ultimately utilizing these components to price a put option through put-call parity. The notebook's resolution, as previously discussed, ensures that the functions used for pricing return the necessary values for this workflow to complete successfully.

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

##  Cox-Ingersoll-Ross (CIR) model On Euribor rates
![image](https://github.com/user-attachments/assets/befc58e0-9fa2-42f1-98f0-6290dd9b0417)



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
