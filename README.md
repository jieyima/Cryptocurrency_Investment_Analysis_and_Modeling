# **Cryptocurrency Investment Analysis and Modeling**


This repository contains the entire analysis and modeling of cryptocurrency performance in the stock market, in the form of Jupyter notebooks.



![CryptocurrencyGeneral](https://user-images.githubusercontent.com/31974451/37227029-ab3a6044-2390-11e8-8728-ccfe6ab07434.png)

# **About**

This is UC Davis BAX452 Machine Learning Autodesk Group Project.

The objective of this project is **to predict 30-days price of the most popular cryptocurrencies** given their historical variations. To achieve this, several regression techniques are explored. In the end, **Gradient Boosting Regressor** yields to the best prediction result for Ripple, and **ExtraTrees Regressor** performs the best for the rest of cryptocurrencies (e.g., Bitcoin, Ethereum, Litecoin, etc.).


Cryptocurrencies mentioned in this Notebook have the following abbreviation:
- Bitcoin (BTC)
- Ethereum (ETH)
- Litecoin (LTC)
- Bitcoin Cash (BCH)
- Ripple (XRP)
- Monero (XMR)
- Zcash (ZEC)


# **How to Navigate this Notebook**

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


# **Visualization Excerpts**

### 1. Bitcoin Price Simulation (2017.1 - 2018.3)
This notebook used plotly to visually show bitcoin stock price during the period from Jan. 2017 to Mar. 2018. This plot illustrates the moving average, volume of transaction, opening price, Bollinger Bands, as well as whether the price increases (blue) or decreases (grey).

![plotly](https://user-images.githubusercontent.com/31974451/37195543-21878f06-2328-11e8-9d24-68d488b85e9d.png)

### 2. Heatmap

Below is a correlation heatmap between eight most popular cryptocurrencies. One of the interesting findings is that all of them have a **highly positive correlation coefficience** (≥0.75), indicating all the cryptocurrencies  generally move in the same direction together along with the market.

Monero has the highest correlation coefficient of more than 0.85 with other cryptocurrencies. If the stocks of Bitcoin/Ethereum/Litcoin/Zcash pick up drastically, it is most likely that Monero will experience a similar boost as its fee-driven income picks up and positive earnings reports encourage investors.

Source: [How does correlation affect the stock market? | Investopedia](https://www.investopedia.com/ask/answers/021716/how-does-correlation-affect-stock-market.asp#ixzz59EdIHIh9)


![heatmap](https://user-images.githubusercontent.com/31974451/37195336-3f9ac86a-2327-11e8-8a67-09031834d063.png)

**Investment Advice:** The principal is that **inclusion of negatively correlated assets in a portfolio allows individuals to reduce the overall risk while still allowing for a positive return**. Therefore, to be able to build a diversified portfolio, investors are **not** advised to put all their money into cryptocurrencies market, rather they should diversify their assets into stock market, mutual funds and bank savings.




### 3. 30-days Bitcoin Price Prediction

![bitcoin prediction](https://user-images.githubusercontent.com/31974451/37195307-20924fce-2327-11e8-9027-98f854448a93.png)

**Investment Advice:**
Our 30-days forecast of bitcion price begins from Feb 25 2018, during which the predicted price is still volatile. Downward trending follows a short-term increasing momentum. Investors need to be cautious with the drastic price fluctuation as the price has already gone very high to a point of nearly $1,9000. **A short-term put option** and **a long-term call option** could be the potential preference of investors.
