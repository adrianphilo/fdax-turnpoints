# fdax-turnpoints
using an LSTM model to learn patterns from FDAX trade flow data to predict turning points


##Pattern Recognition and Trading Strategies in FDAX using LSTM Deep Learning

This repository contains source code, results, and analyses conducted as part of a master's thesis on predicting turning points in FDAX trading.

###Project Overview

This work investigates the extent to which a Long Short-Term Memory (LSTM) network can be trained on microstructure data of the FDAX to identify turning points in the daily market trend. A key focus is the hypothesis that the collective trading behavior of market participants can be represented as recurring patterns within the trade data.


### Methodology

The analysis is based on trade data from the FDAX, collected via an API. Twenty derived features were used to represent trading behavior in the short and medium-term past. The performance of the LSTM model was evaluated with varying training data sizes to test its generalization ability. The results were subsequently assessed in a simulated trading environment (backtesting) to measure the profitability of the developed trading strategy.

### Key Findings
The results show that the LSTM model is capable of learning the trigger patterns on the training data with near-perfect accuracy. Tests on unseen data confirm that a reliable prediction of turning points on "normal" trading days is possible. The work demonstrates that simple trading strategies can yield positive results, even when faced with the complex challenges of extreme market conditions.


### Contents
notebooks/: Jupyter notebooks that document the entire process from data preparation to model training.

Data_Preprocessing.ipynb: Scripts for processing raw data into standardized blocks and features.

LSTM_Model_Training.ipynb: Code for the model architecture, training, and evaluation.

results/: Directories and files containing the modeling results.

sheets/: Tables with performance metrics (e.g., Precision, Recall, F1-Score).

charts/: Graphs for visualizing model predictions and backtesting results.

logs/: Training logs documenting the progression of accuracy and loss.
