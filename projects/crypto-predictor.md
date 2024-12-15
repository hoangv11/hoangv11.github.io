---
layout: project
type: project
image: img/CryptoPredictionGraph.png
title: "Crypto Trading Bot & Predictor"
date: 2023
published: true
labels:
  - Python
  - Machine Learning
  - Data Science
  - APIs
summary: "Crypto Trading Bot leveraging machine learning techniques to forecast cryptocurrency stock trends and make trades"
---

## Overview

This project involved designing a Crypto Trading Predictor and Bot that leverages machine learning algorithms to forecast cryptocurrecny market trends and executing trades automatically based off of the trends. My primary goal of the bot was to provide both an efficient as well as an automated solution to navigate through the very highly volatile cryptocurrency market. For this specific bot, I had it execute trades on some popular crypocurrencies such as Bitcoin, Ethereum, Tether, Solana and XRP. I chose these coins because due to their higher liquidity, market influence as well as more readily available data, it was much easier to make predictions on their trends as compared to smaller coins which reduced some of the risks that comes with crypto and stock trading. By analyzing the historical data, trading volumes, and volatility of these coins, the bot was able to predict prive movements and generate predictions that informed the bot's trading decisions. It took these predictions to make buy or sell decisions in real time while optimizing for profit and managing risks. 

The architecture of the bot is built around 4 steps before executing a trade. First it starts with data ingestion where it takes real time data. The system was connected with an API from Kraken to gather market data, including prices, volume and order book depth. It then processes and cleans that data by handling missing values, removing outliers and creating more consistent formats which allows for much more accurate data analysis. With that data, it beings to make machine learning based predictions. Using historical and real-time data, the machine implements alogirhtms such as Linear Regression or Long Short-Term Memory (LSTM) networks or some tree based models in order predict short term price changes and outputting signals to either Buy, Sell or Do Nothing/Hold. Finally, the bot then performs automated actions based on signals and performs market, limit or stop-loss orders. For example, if the bot predicts that Ethereum would have a 5% price increase, it will place a buy order while setting a stop loss at around 3% below the purchase price for proper risk management. 

## My Contribution

Due to this being a solo project I made for fun, I was the primary developer and architect for the entire project whether it be the design or the implmentations. My contributions included:

1. Data Pipeline and Preprocessing:

   - Designed a data pipline to ingest both real-time and historical data from Kraken API, including the price history and trading volumes of 5 popular crypocurrencies.

   - Developed preprocessing algorithms to clean up data allowing for more meaningful data analysis that is compatible with certain machine learning models

2. Machine Learning Model Development:

   - Implemented predictive machine learning models such as LSTM netoworks and Linear Regression to make decisions based on short term movement.
  
   - Tuning hyperparemeters such as Root Mean Squared Error (RMSE) to optimize performance of learning models setting boundaries for the learning models. RMSE is a means of measure to gives weight to larger errors by     
     squaring the differences before averaging the errors emphasizing larger deivations which is important in order to maintain accuracy. 

3. Trading Logic and Risk Management:

   - Incorporated risk management features such as stop-loss orders and position size limits to mitigate potential losses.
  
   - Developed the bot's decision-making logic to execute trades based on model outputs creating signals that determined the bot's actions. 

## Lessons Learned and Skills Acquired

1. Machine Learning

2. System Design, Optimization and API Integration

3. Crypto Market Dynamics




