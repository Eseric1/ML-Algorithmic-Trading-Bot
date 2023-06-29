# ML-Algorithmic-Trading-Bot
This repository contains the code and data for a machine learning project that aims to create an algorithmic trading bot that can predict the movements of an exchange-traded fund based on historical data and sentiment analysis.

## Data
The provided CSV file contains open, high, low, close, and volume (OHLCV) data for a Morgan Stanley Capital International (MSCI)–based emerging markets exchange-traded fund (ETF) that iSharesLinks to an external site. issued. Investments in emerging markets make up an important aspect of a well-diversified investment portfolio.
## Models
Two models were built and evaluated for this project: a baseline model and a tuned model. Both models were logistic regression models, which are commonly used for binary classification problems.
- Baseline model used the default parameters of the sklearn LogisticRegression class. 
- Tuned model used a grid search with cross-validation to find the optimal parameters.

The models were trained on the training set and evaluated on the testing set using various metrics, such as accuracy, precision, recall, f1-score, confusion matrix, and classification report.

## Results
The baseline model performed slightly better than the tuned model in terms of precision, recall, and f1-score for both classes. However, the difference was not very significant and the accuracy remained the same at 0.55. This suggests that the tuned model did not improve much on the performance of the baseline model and may have overfitted or underfitted the data. The baseline model also had a higher macro average f1-score, which means that it was more balanced in handling both classes. However, both models had low f1-scores for the negative class, which indicates that they were not very good at predicting the downward movements of the market.


## Conclusion
The results of this project show that using historical prices and sentiment analysis to predict the movements of the Morgan Stanley Capital International (MSCI)exchange-traded fund (ETF), is not very effective, as both models had low accuracy and f1-scores.

To make these models better we can

- Explore different sources and types of data that could provide more insights into the market behavior
- Try different models and algorithms that could better capture the nonlinear relationships in the data
- Tune more parameters and using more validation techniques to avoid overfitting or underfitting