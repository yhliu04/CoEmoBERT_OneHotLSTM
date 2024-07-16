# 通过大众情绪分析和多元时间回归预测股票趋势变化

## Introduction
在金融市场中，股票价格的波动不仅受经济数据和市场趋势的影响，还受到投资者情绪和公众舆论的影响。为了更准确地预测股票价格的变化，我们提出了一种结合大众情绪分析和多元时间序列回归的预测方法。我们的项目旨在建立一个综合数据集，并开发一个多元时间序列预测模型，用于预测股票的未来趋势。

### 数据来源
我们的数据集主要来源于两个平台：
1. **StockTwits**：一个专注于股票和交易的社交媒体平台，用户在此分享他们对股票的看法和情绪。我们从中提取用于情感分析的文本数据。
2. **Yahoo Finance**：一个提供股票价格、财务报表和市场数据的平台。我们从中获取股票价格的时间序列数据。

### 模型概述
我们的方法包括以下几个步骤：
1. **文本数据处理与情感分析**：
   - 使用NLP技术与大语言模型对StockTwits上的用户评论进行处理，提取情感向量。这些向量代表了用户对某只股票的情感分布，如乐观、悲观或中立。
   - 将这些情感向量转化为可用于时间序列分析的形式。

2. **数字数据处理与模型预测**：
   - 获取目标股票在过去一段时间内的价格数据，包括开盘价、收盘价、最高价、最低价和交易量等。
   - 将提取的情感向量与股票价格的历史数据结合，训练一个时间序列预测模型，进行股票价格预测

3. **模型验证与评估**：
   - 使用交叉验证和滚动预测方法验证模型的性能，确保其在不同时间段上的稳定性和准确性。
   - 评估模型的预测效果，并与传统的预测方法进行比较，验证其优势。

### 应用与展望
通过将情感分析与时间序列预测相结合，我们的模型可以更准确地捕捉市场情绪对股票价格的影响。这种方法不仅可以用于股票价格的预测，还可以扩展到其他金融产品，如期货、外汇和加密货币等。

## Reference
https://github.com/adlnlp/StockEmotions/tree/main



# Predicting Stock Trend Changes through Public Sentiment Analysis and Multivariate Time Series Regression

## Introduction
In the financial market, stock price fluctuations are influenced not only by economic data and market trends but also by investor sentiment and public opinion. To more accurately predict stock price changes, we propose a method that combines public sentiment analysis and multivariate time series regression. Our project aims to establish a comprehensive dataset and develop a multivariate time series prediction model to forecast future stock trends.

### Data Sources
Our dataset primarily comes from two platforms:
1. **StockTwits**: A social media platform focused on stocks and trading, where users share their opinions and sentiments about stocks. We extract text data for sentiment analysis from this platform.
2. **Yahoo Finance**: A platform that provides stock prices, financial statements, and market data. We obtain time series data of stock prices from this source.

### Model Overview
Our approach includes the following steps:
1. **Sentiment Analysis**:
   - Using the BERT model to process user comments on StockTwits and extract sentiment vectors. These vectors represent the sentiment distribution of users towards a particular stock, such as optimistic, pessimistic, or neutral.
   - Transforming these sentiment vectors into a format suitable for time series analysis.

2. **Time Series Data Processing**:
   - Collecting historical stock price data, including open price, close price, high price, low price, and trading volume.
   - Preprocessing and normalizing the data to ensure its suitability for the subsequent modeling process.

3. **Multivariate Time Series Prediction Model**:
   - Designing and training a Long Short-Term Memory (LSTM) network capable of handling time series data and capturing long-term dependencies.
   - Combining the extracted sentiment vectors with historical stock price data as inputs to the LSTM model to predict the next time point's stock price.

4. **Model Validation and Evaluation**:
   - Using cross-validation and rolling prediction methods to validate the model's performance, ensuring its stability and accuracy over different time periods.
   - Evaluating the prediction results and comparing them with traditional prediction methods to verify the model's advantages.

### Applications and Prospects
By integrating sentiment analysis with time series prediction, our model can more accurately capture the impact of market sentiment on stock prices. This approach can be applied not only to stock price prediction but also to other financial products, such as futures, forex, and cryptocurrencies.

## Reference
https://github.com/adlnlp/StockEmotions/tree/main
