# Luke_portfolio

## [Project 1 - Option Trading and Analysis](https://github.com/lbianculli/options_nb)

A tutorial notebook that examines how options data can be scraped using Python and how that data can be implemented for trading strategies. 

This walkthrough starts by first scraping put and call pricing data for commonly-traded index equities (SPY, QQQ, etc.). After the data is scraped, pandas DataFrames are put together for puts and calls. From there, we explore how to turn that code into a Class and expand upon it to implement trading strategies such as credit spreads and iron condors. Finally, we run through examples before delving into some analysis that examines the efficacies of potential strategies. By the end of this notebook, I hope that it is clearly conveyed how options can be traded in an everyday account to augment a portfolio and how such strategies would be implmented and analyzed with Python.


## [Project 2 - US Equity Machine Learning Research](https://github.com/lbianculli/us_equity_analysis)

This repository will walk through a holistic process of preprocessing and premodeling data in preparation for feeding a machine learning algorithm. After premodeling various models are explored, the best of which is thoroughly evaluated. The files within the repo, which follow standard steps for machine learning analysis, can be broken down as follows:

1. Preprocessing: Perform fundamental data preprocessing starting with previously-scraped US pricing, macro, and fundamental data. This short notebook walks through how to deal with missing values, handling outliers, scaling data, and augmenting data with additional metrics based on data collected from financial statements.

2. Premodeling: A longer notebook in which many of the steps may also be classified as preprocessing. The focus of this code is to specifically prepare our data for feeding through a Machine Learning model in Python. This notebook contains 500-1000 lines of code focused on: examining and visualizaing linear interactions, measuring feature importance, and reducing our feature space.

3. Model Selection: Split data into train, test, and holdout data and use SKLearn's GridSearch class to determine the best model and perform hyperparameter tuning.

4. Model Evaluation: With the fully trained model and holdout data available, this notebook starts by confirming efficiacy of the model on the holdout data, after which the performance of the model is analyzed according to various metrics such as F1 score, confusion matrix, and the ROC/AUC score. Finally, using optimal thresholds determined by the ROC/AUC curve, securities that would have been chosen by the model in a prior period are measured and evaluated against returns of the S&P500 ETF during the same time period.

## [Project 3 - US Equity Statistical Analysis (R)](https://github.com/lbianculli/us_equity_stat_analysis)

![](/images/factor_corr_mat.png)

This repository runs through a host of analyses examining the statstical properties and structure of US equity returns and how they relate to a portfolio of assets, starting with data collected during a machine learning analysis of US equities (Project 2). Unlike the rest of the projects outlined here, this repo will use strictly R code. 

We begin by calculating the distribution of monthly returns for large-cap US equities and compare them to the normal and T distributions. Then we delve deeper into univariate factor analysis of returns bucketing data by factors that can be examined on the income statement, balance sheet, and cash flow statement. We then visualize the performance of these factors via returns, volatility, and sharpe ratio. Then we rank the factors that performed the best over the period of time the data was collected before finally looking at the correlation for top-performing factors.

## Project 4 - TBD
