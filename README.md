# XAI-Stock-Market-Prediction

This repository presents a comprehensive approach to forecasting Apple Inc. (AAPL) stock price movements using deep learning models, technical indicators, and Explainable AI (XAI) techniques. The project aims to predict stock price trends based on historical data and provide interpretable insights into the model's decision-making process.

## Overview

We implemented three distinct deep learning architectures to forecast AAPL price movements, with a focus on the preceding 90 days of data. The result are below:

- **LSTM (Long Short-Term Memory)** - MAE: 0.0887
- **GRU (Gated Recurrent Units)** - MAE: 0.0756
- **LSTM-GRU Hybrid** (the most effective ) - MAE: 0.0518

We used technical indicators such as the Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) to help the model make better predictions and SHapley Additive exPlanations (SHAP) to further interpret them, providing insights into each feature's contributions. To generate their textual explanations, we integrated GPT-2.

## Repository Structure

```plaintext
XAI-Stock-Market-Prediction/
│
├── code/
│   ├── Checking the environment/
│       └── main.ipynb         
│   ├── Preprocessing data/
│       └── main.ipynb     
│   ├── Designing multiple architectures/
│       └── main.ipynb   
│   ├── Comparing the model with naive forecast/
│       └── main.ipynb  
│   ├── Further analyzing on the data to understand the results of the model/
│       └── main.ipynb  
│   ├── Transitioning from black-box to XAI/
│       └── main.ipynb   
│   └── Takeaways/
│       └── main.ipynb  
│
├── database/
│   └── aapl_stock_data.csv         # Historical stock data
│
├── pickles/
│   ├── Optuna/
│       └── optuna_study_lstm.pkl
│       └── optuna_study_gru.pkl
│       └── optuna_study_lstm_gru.pkl           
│   └── Weights/
│       └── best_model_lstm_after_optuna.h5
│       └── best_model_gru_after_optuna.h5
│       └── best_model_hybrid.h5 
│
└── README.md                       # Project documentation
```

## Requirements

Before running the code, ensure that you have installed the followings:

```plaintext
pip install keras tensorflow pandas pandas-ta numpy seaborn matplotlib yfinance scikit-learn optuna shap 
```


## How to Run

Clone the repository with the following commands in a Command Prompt:

```plaintext
git clone https://github.com/nb71325/XAI-Stock-market-prediction.git
cd XAI-Stock-market-prediction
```
