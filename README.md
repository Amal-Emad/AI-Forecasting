# Time Series Forecasting with LSTM

## Overview
This project implements time series forecasting using Long Short-Term Memory (LSTM) networks, focusing on predicting the closing prices of the S&P 500 Index.

## Requirements
- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Plotly

You can install the required packages using pip:


## File Structure
- `S&P_500_Index_Data.csv`: The dataset containing historical data of the S&P 500 Index.
- `time_series_forecasting_lstm.ipynb`: The Jupyter Notebook containing the code implementation.
- `README.md`: This file providing an overview of the project.

## Data Preprocessing
### Reading Data
Read the S&P 500 Index data from the CSV file.
### Exploratory Data Analysis (EDA)
Perform EDA to understand the dataset's characteristics.
### Standardizing Data
Standardize the closing prices using `StandardScaler`.
### Creating Time Sequences
Split the data into training and testing sets and create sequences for LSTM modeling.

## LSTM Model Training
### Model Architecture
Define an LSTM autoencoder model using TensorFlow's Keras API.
### Model Training
Train the LSTM model on the training data with early stopping.
### Plot Training Loss
Visualize the training and validation loss to monitor the model's performance.

## Anomaly Detection
### Calculate Loss
Calculate the Mean Absolute Error (MAE) loss between actual and reconstructed sequences.
### Threshold Calculation
Determine a threshold for anomaly detection based on the training loss distribution.
### Detect Anomalies
Identify anomalies by comparing the loss values to the threshold.
### Visualize Anomalies
Plot the test loss, threshold, and anomalies to visualize detected anomalies.

## Results Visualization
### Plot Test Loss and Threshold
Visualize the test loss and threshold over time to assess anomaly detection performance.
### Plot Anomalies on Close Price Chart
Plot original closing prices along with detected anomalies to visualize their impact on the S&P 500 Index.

## Conclusion
Summarize key findings and suggest potential areas for further improvement.

