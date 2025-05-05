# XAI-Stock-Market-Prediction

This repository presents a comprehensive approach to forecasting Apple Inc. (AAPL) stock price movements using deep learning models, technical indicators, and Explainable AI (XAI) techniques. The project aims to predict stock price trends based on historical data and provide interpretable insights into the model's decision-making process.

## 🔍 Overview

The project explores three distinct deep learning architectures to forecast AAPL price movements, with a focus on the preceding 90 days of data. The models tested include:

- **LSTM (Long Short-Term Memory)**
- **GRU (Gated Recurrent Units)**
- **LSTM-GRU Hybrid** (identified as the most effective model)

Incorporating technical indicators such as the Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) enhances the model's ability to mimic actual price movements. To further interpret the model's predictions, SHAP (SHapley Additive exPlanations) values are utilized, providing insights into feature contributions.

Additionally, the project integrates GPT-2 to generate textual explanations, aiding in understanding the optimal timing for stock investments.

## 📁 File Structure

