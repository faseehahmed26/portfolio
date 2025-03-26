---
title: "Analysis on Various Commodities"
description: "Time series analysis and prediction using LSTM networks"
dateString: Oct 2022
draft: false
tags: ["Deep Learning", "LSTM", "Web Scraping", "Time Series", "Python", "TensorFlow", "Keras", "Data Analysis", "Visualization"]
showToc: false
weight: 206
cover:
   image: "projects/commodity/commod.jpeg"
--- 
##### 🔗 [GitHub](https://github.com/faseehahmed26/Commodities-Investing.com)
##### 🔗 [Scraper Code](https://github.com/faseehahmed26/Commodities-Investing.com/blob/main/commoditiesScraper.py)

## Description

I developed a comprehensive commodities analysis system that combines web scraping, data visualization, and deep learning to predict price movements across multiple markets. The project focused on six major commodities: Gold, Silver, Crude Oil, Brent Oil, Natural Gas, and Copper.

First, I created a custom web scraper using Beautiful Soup to extract historical price data from Investing.com, allowing flexible date range selection. This data collection tool enabled me to compile 10 years of daily price information for analysis.

Through extensive exploratory data analysis, I identified significant cross-commodity correlations:
- Strong positive correlation between Crude Oil, Brent Oil, and Natural Gas prices
- Positive correlation between Gold, Silver, and Copper prices
- Interconnected relationships between energy and metals markets

For the predictive component, I implemented Long Short-Term Memory (LSTM) neural networks using TensorFlow and Keras to forecast future price movements. The models achieved impressive accuracy with low Mean Squared Error scores across all commodities (Gold: 0.27, Silver: 0.40, Crude Oil: 0.34, Brent Oil: 0.27, Natural Gas: 0.35, Copper: 0.32).

This project demonstrates advanced abilities in time series analysis, web scraping, data visualization, and deep learning implementation. The insights derived provide valuable market intelligence for investors and commodity traders, while the LSTM models offer a foundation for algorithmic trading strategies.