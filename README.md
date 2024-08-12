# Understanding Concept of Financial Engineering 

File : Analyzing pirice stocks and crypto \\ need to make a table 

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
