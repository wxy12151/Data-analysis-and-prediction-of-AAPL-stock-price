[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-f059dc9a6f8d3a56e377f745f24479a46679e63a5d9fe6f495e02850cd0d8118.svg)](https://classroom.github.com/online_ide?assignment_repo_id=6534887&assignment_repo_type=AssignmentRepo)
# Setup

## Environment: 

CPU: Intel 8- Core i7-11800

GPU: RTX 3060

## External libraries:

keras

pandas

sklearn

seaborn

statsmodels

tensorflow

pymongo[srv]

# 1. Brief introduction

This project obtains AAPL historical stock data from April 2017 to April 2021 to predict the closing price of the trading day in May 2021. The purpose of this research is to examine and analyze the variations that occur when the multi-step output LSTM is trained to predict AAPL closing prices using only closing prices and using that with adding auxiliary properties. Specifically, auxiliary properties contain Nasdaq and Dow Jones stock index, Google Trends and USD/CNY. 

## Task 1: Data Acquisition

1. Stock APPL Data Acquisition by API
2. Stock Apple Data Acquisition downloaded from the Internet
3. Nasdaq share index by API using the same datetime as APPL stock
4. Dow Jones share index by API using the same datetime as APPL stock
5. Google Search APPLE trend 2017/4/1-2021/6/1 weekly from Internet
6. USD/CNY 2017/4/1-2021/6/1 weekly from Internet

## Task 2: Data Storage

1. Store and retrieve data.

2. Upload to MongoDB and test the API.

## Task 3: Data Preprocessing

Task 3.1: Clean the data from missing values and outliers, if any

3.1.1 Using Z score to check if there are outliers in AAPL stock dataset and cap them

3.1.2 Using Z score to check if there are outliers in Google Trends and USD/CNY and cap them

3.1.3 Count the number of missing values in each column of the dataset.

Task 3.2: Data integration

Task 3.3: Data Visualization

3.3.1 AAPL Boxplots monthly

3.3.2 Explore dependency on day of the week and month via carpet plot/heatmap

3.3.3 Autocorrelation of AAPL Close

Task 3.4: Data Normalization and Dimensionality reduction

## Task 4: Data Exploration

Task 4.1: Trend, seasonality and random noise

Task 4.2: Proximity Measures

Task 4.3: Data Relationships - spearman correlations and scatter plots

Task 4.4: Hypothesis Testing

Task 4.4.1 AAPL Close price rise/fall vs AAPL Volume rise/fall --> Dependent

Task 4.4.2 AAPL Close price rise/fall vs with/without pandemic --> Independent

## Task 5: Inference

5.1 Using LSTM with 2 layers to train the dataset.

A: using only time series of stock prices

B: using the time series of stock prices and the auxiliary data

5.2 Prediction one-month trading days of AAPL closing prices

5.3 Evaluation Metrics Implementation

5.3.1 STATISTICAL PERFORMANCE： MSE MAE R-squared

5.3.2 JOINT PLOTS

5.3.3 RESIDUAL DISTRIBUTION PLOTS

# 2. Organization of the files

## 2.1. auxiliary

store the auxiliary datasets: Nasdaq, Dow Jones indicates, Google Trends, USD/CNY

## 2.2. stock

store the AAPL stock dataset

## 2.3. image

which is used to save the plots running in the code(without plot.show())

# 3. Run the code

### Open the "assignment.ipynb"--> run the functions defined before main()-->run main()





















