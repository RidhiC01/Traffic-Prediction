# Traffic-Prediction
A deep learning approach to forecast hourly traffic volume using LSTM networks.

# Project Overview
This project demonstrates time series forecasting for traffic volume prediction using deep learning. The workflow covers data preprocessing, feature engineering, model building with LSTM layers, and evaluation of the results through loss metrics and visualization.

# Dataset
Source: Traffic data CSV file (traffic.csv)

# Columns:

DateTime: Timestamp of the record

Junction: Identifier for the traffic junction

Vehicles: Number of vehicles counted

ID: Unique record identifier

The dataset is enhanced with additional time-based features such as hour, day, month, weekday, and rolling statistics for improved predictive performance.

# Methodology
Data Preprocessing: Handling missing values, feature engineering (hour, day, month, weekday, is_weekend, lag features, rolling averages)

# Model Architecture:

Two LSTM layers (64 and 32 units)

Dropout layer for regularization

Two Dense layers (16 units and 1 output)

# Training:

20 epochs, batch size of 32

Validation on a held-out test set

# Evaluation:

Loss values tracked for both training and validation

Visualization of actual vs. predicted traffic counts

# Results
Model Performance: The LSTM model achieved low validation loss, indicating good predictive accuracy.

Visualization: The plot below shows actual vs. predicted traffic volume, demonstrating the model's effectiveness in capturing temporal patterns.

# Getting Started
Prerequisites
Python 3.10+

Required libraries: numpy, pandas, scikit-learn, matplotlib, tensorflow or keras

Installation
bash
pip install numpy pandas scikit-learn matplotlib tensorflow
Usage
Clone the repository and navigate to the project directory.

Place traffic.csv in the input directory.

Run the main notebook or script to preprocess data, train the model, and visualize results.

# Project Structure

traffic-1.ipynb        # Main Jupyter notebook

traffic.csv            # Dataset file

README.md              # Project documentation
