XAI-Stock-Market-Prediction
This repository presents a comprehensive approach to forecasting Apple Inc. (AAPL) stock price movements using deep learning models, technical indicators, and Explainable AI (XAI) techniques. The project aims to predict stock price trends based on historical data and provide interpretable insights into the model's decision-making process.

🔍 Overview
The project explores three distinct deep learning architectures to forecast AAPL price movements, with a focus on the preceding 90 days of data. The models tested include:

LSTM (Long Short-Term Memory)

GRU (Gated Recurrent Units)

LSTM-GRU Hybrid (identified as the most effective model)

Incorporating technical indicators such as the Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) enhances the model's ability to mimic actual price movements. To further interpret the model's predictions, SHAP (SHapley Additive exPlanations) values are utilized, providing insights into feature contributions.

Additionally, the project integrates GPT-2 to generate textual explanations, aiding in understanding the optimal timing for stock investments.

📁 File Structure
graphql
Copy
Edit
XAI-Stock-Market-Prediction/
│
├── code/
│   ├── data_preprocessing.py          # Scripts for data cleaning and feature engineering
│   ├── model_training.py              # Training routines for LSTM, GRU, and hybrid models
│   ├── shap_analysis.py               # SHAP value computation and visualization
│   └── gpt2_integration.py            # GPT-2 integration for generating textual explanations
│
├── database/
│   └── aapl_stock_data.csv            # Historical AAPL stock data
│
├── pickles/
│   ├── trained_model.pkl              # Serialized trained model
│   └── shap_values.pkl                # Serialized SHAP values
│
└── README.md                         # Project overview and instructions
🛠️ Requirements
To run the project, ensure you have the following Python packages installed:

numpy

pandas

matplotlib

seaborn

tensorflow

keras

shap

transformers

These dependencies can be installed using pip:

bash
Copy
Edit
pip install -r requirements.txt
🚀 Usage
Clone the Repository

bash
Copy
Edit
git clone https://github.com/nb71325/XAI-Stock-market-prediction.git
cd XAI-Stock-market-prediction
Prepare the Data

Place the historical AAPL stock data CSV file in the database/ directory.

Preprocess the Data

Run the data preprocessing script to clean and prepare the data:

bash
Copy
Edit
python code/data_preprocessing.py
Train the Models

Train the LSTM, GRU, and hybrid models:

bash
Copy
Edit
python code/model_training.py
Analyze SHAP Values

Compute and visualize SHAP values to interpret model predictions:

bash
Copy
Edit
python code/shap_analysis.py
Generate Explanations with GPT-2

Use GPT-2 to generate textual explanations for model predictions:

bash
Copy
Edit
python code/gpt2_integration.py
📈 Results
The LSTM-GRU hybrid model demonstrated the best performance in forecasting AAPL price movements. The integration of RSI and MACD indicators improved the model's accuracy in mimicking actual price trends. SHAP analysis provided valuable insights into feature importance, while GPT-2 generated coherent textual explanations, aiding in understanding the optimal investment timing.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

📞 Contact
For questions or contributions, please open an issue or submit a pull request on the GitHub repository.

