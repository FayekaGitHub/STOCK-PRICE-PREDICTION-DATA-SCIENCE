# Stock Price Prediction Using LSTM

## Overview

This project demonstrates how to predict stock prices using Long Short-Term Memory (LSTM) networks,a type of Recurrent Neural Network (RNN) that is well-suited for sequential data.
The primary objective is to forecast future stock prices based on historical price data.

### Data Preprocessing
#### Data Preparation:
The data is cleaned to retain only relevant columns: Date, Open, High, Low, Close, Adj Close, and Volume.
The closing prices are scaled to a range of 0 to 1 using MinMaxScaler to normalize the data for better performance of the LSTM model.
#### Creating LSTM Data:
A function is defined to create sequences of data for LSTM input.
This function generates input-output pairs where the input is a sequence of previous time steps and the output is the next time step’s price.

### Model Building and Training
#### Model Architecture:
A Sequential model is created with LSTM layers for capturing temporal dependencies, Dropout layers to reduce overfitting, and a Dense layer for prediction.
The model is compiled with the Adam optimizer and Mean Squared Error loss function and trained.
### Results
The final output is a DataFrame containing the forecasted stock prices for the next 30 days.

#### DISCLAIMER: 
This stock market price prediction code is developed for educational purposes only. 
It is not intended for real-time trading or financial decision-making.
The predictions made by this code are based on historical data and may not be accurate or reliable for future market conditions.
