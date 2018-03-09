# Cryptocurrency_Investment_Analysis_and_Modeling


This repository contains the entire analysis and modeling of cryptocurrency performance in the stock market, in the form of Jupyter notebooks.

![CryptocurrencyWordMap](https://user-images.githubusercontent.com/31974451/37195011-e684cb46-2325-11e8-994e-bf411f1c97fe.jpg)

## How to Navigate this Notebook

Here is the table of content for you to navigate:

<a id="0"></a>
[1. Prepare Data Set](#1)
 - [Load Python Packages](#1-1)
 - [Load and Prepare Data Set](#1-2)

[2. Data Quality Assessment](#2)
 - [Check Missing Values](#2-1)
 - [Check Duplicated Values](#2-2)

[3. Exploratory Data Analysis and Feature Selection](#3)
 - [1.Check market capitalization and transaction volume for each cryptocurrency we choose](#3-1)
 - [2.Check opening and closing price for each of the cryptocurrency](#3-2)
 - [3.Moving averages](#3-3)
 - [4.Check high, low, and average price for each cryptocurrency](#3-4)
 - [5.Check return ratio](#3-5)
 - [6.Candlestick charts using Plotly (BitCoin)](#3-6)
 - [7.Check Pearson correlation coefficient to prove if BitCoin price influences price of other cryptocurrencies](#3-7)
 - [8.Feature selection for prediction models](#3-8)

[4. Building Models - Predicting Price for Cryptocurrencies](#4)
 - [Prepare Data for Models](#4-1)
 - [Applying Machine Learning Models](#4-2)
 - [Prices Prediction](#4-3)

[5. Conclusion - Which Cryptocurrencies to Invest](#5)
 - [Prices Prediction](#5-1)
 - [Result Summary](#5-2)
 - [Interesting Findings](#5-3)

[6. Limitations](#6)

[7. Future Work](#7)

[8. Reference](#8)

## About
In this Notebook, I am investigating in the most popular cryptocurrencies, the following abbreviation:
- Bitcoin (BTC)
- Ethereum (ETH)
- Litecoin (LTC)
- Bitcoin Cash (BCH)
- Ripple (XRP)
- Monero (XMR)
- Zcash (ZEC)


## Some cool Visualizations

### 1. Bitcoin Price Simulation (2017.1 - 2018.3)
Using plotly to draw bitcoin stock price during the period from Jan 2017 to Mar. 2018. The plot shows the opening price, moving average, volume of transaction, Bollinger Bands, as well as whether the price increases (blue) or decreases (grey).

![plotly](https://user-images.githubusercontent.com/31974451/37195543-21878f06-2328-11e8-9d24-68d488b85e9d.png)

### 2. Heatmap

Below is a correlation heatmap among 8 cryptocurrencies. One of the interesting findings is that all of them have a high correlation (higher than 0.75), and Litcoin and Monero have the highest correlation with all other cryptocurrencies. This phenomenon indicates that if the stocks of Bitcoin, Ethereum pick up drastically, it is highly likely that Litcoin/Bitcoin Cash/Zcash will experience a similar boost as its fee-driven income picks up and positive earnings reports encourage investors.

[Source: How does correlation affect the stock market?|Investopedia](https://www.investopedia.com/ask/answers/021716/how-does-correlation-affect-stock-market.asp#ixzz59EdIHIh9)



![heatmap](https://user-images.githubusercontent.com/31974451/37195336-3f9ac86a-2327-11e8-8a67-09031834d063.png)



### 3. 30-days Bitcoin Price Prediction
![bitcoin prediction](https://user-images.githubusercontent.com/31974451/37195307-20924fce-2327-11e8-9027-98f854448a93.png)
