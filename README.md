## FDAX Turnpoints
### Pattern Recognition and Trading Strategies in FDAX using LSTM Deep Learning

This repository contains source code, results, and analyses conducted as part of a thesis on predicting turning points in FDAX trading.

### Project Overview

This work investigates the extent to which a Long Short-Term Memory (LSTM) network can be trained on microstructure data of the FDAX to identify turning points in the daily trade flow data. 
A key focus is the hypothesis that the collective trading behavior of market participants can be represented as recurring patterns within the trade data.

### Key Findings

The results show that the LSTM model is capable of learning the trigger patterns on the training data with near-perfect accuracy. 
Tests on unseen data confirm that a reliable prediction of turning points on "normal" trading days is possible. 
The work demonstrates that simple trading strategies can yield positive results.


### Contents of the Subdirectories

#### [results: contains the results of the backtesting test series](results)

Results overview of the limit strategie with the 67 days model.

| Model | Total Trades | Successful Trades (Hits) | Precision of Performance | Total Profit/Loss (Points) |
| ----- | ----- | ----- | ----- | ----- |
| **HI 67** | 107 | 48 | 0.449 | 1119,3 |
| **LO 67** | 70 | 37 | 0.529 | 669,2 |

#### [charts: Graphs for visualizing model predictions and backtesting results](charts)

As an example the prediciton chart and the limit strategie results of 83 days modell is shown:\
Limit  , HI 83 , precision : 0,667 , sum_pl ; 134,9, max_pl : 72,9 : min_pl , -5,0\
Limit  , LO 83 , precision : 0,800 , sum_pl : 63,1 , max_pl : 19,3 , min_pl : 0,0\
![Prediciton chart 83 days modell](charts/testseries_1/0924/plt_24_09_24_d83a.png)


#### [notebooks: Colab Jupyter notebooks for data preparation, training and backtesting with charts output](notebooks)

#### [logs: Training logs documenting the progression of accuracy and loss](logs)

#### [data_example: Contains some data files that are used and build in the data preparation](data_example)
