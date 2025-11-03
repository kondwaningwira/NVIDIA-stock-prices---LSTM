# NVIDIA-stock-prices---LSTM
NVIDIA Stock Price Prediction using LSTM
📘 Project Overview

This project uses a Long Short-Term Memory (LSTM) model — a type of recurrent neural network (RNN) — to predict future NVIDIA (NVDA) stock closing prices based on historical data. The project demonstrates time series forecasting using deep learning and serves as an introduction to financial data modeling.

📊 Dataset

Source: Historical stock data for NVIDIA (NVDA)

Duration: August 20, 2019 – August 20, 2024

Features used: Only the Closing Price column was used for prediction

File: NVDA.csv

⚙️ Project Workflow

Data Loading and Preprocessing

Imported data using pandas

Kept only the closing price

Scaled data using MinMaxScaler for better neural network performance

Time Series Data Generation

Used TimeseriesGenerator from Keras to create sliding windows of 60 days to predict the next day’s price

Model Building

Built an LSTM-based Sequential model using TensorFlow/Keras

Layers:

LSTM

Dropout (to prevent overfitting)

Dense output layer

Training

Model trained on 90% of the dataset

Remaining 10% used for testing

Optimized to minimize Mean Squared Error (MSE)

Evaluation and Visualization

Compared predicted vs. actual prices

Visualized training loss and forecast accuracy using Matplotlib

🧩 Technologies Used

Python 3

TensorFlow / Keras

Pandas

NumPy

Matplotlib

Scikit-learn

📈 Sample Results

The LSTM model learns temporal dependencies in stock prices and generates predictions that closely follow the real price trend.
