# 通过大众情绪分析和多元时间回归预测股票趋势变化
## intrduction
我们的工作主要包括建立一个数据集并形成一个对应的多元时间序列预测模型进行股票趋势的预测。数据集来源主要来自StockTwits（情感分析的文本），Yahoo Finance（股票价格的时间序列），我们利用bert大模型提取文本的情感向量，将其和当前点之前的股票时间序列结合，通过lstm预测下一时刻的股票价格。
我们的工作量主要包括：1.从StockTwits分析用户对于一只股票的评价，并提取情感分布向量2.将情感结合Yahoo Finance上的股票价格时间序列预测接下一段时间内的股票趋势走向
## reference
https://github.com/adlnlp/StockEmotions/tree/main
