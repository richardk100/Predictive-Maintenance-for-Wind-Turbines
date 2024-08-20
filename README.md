# Predictive-Maintenance-for-Wind-Turbines

This project leverages machine learning to predict equipment failures in wind turbines. Using sensor data such as temperature, vibration, and acoustic readings, the model can detect potential failures before they occur, allowing for proactive maintenance and reducing downtime.

## Project Overview

The goal of this project is to build a predictive maintenance system using a RandomForestClassifier. The model uses rolling averages, standard deviations, and raw sensor data to classify whether a wind turbine is likely to fail.

## Dataset

The dataset used in this project contains sensor readings from wind turbines. The key sensors are:

- **Temperature**
- **Vibration**
- **Acoustic Signals**

### Data Preprocessing

- **Date Extraction:** Year, month, day, and weekday features are extracted from the timestamp.
- **Rolling Statistics:** Rolling averages and standard deviations are computed to capture trends over time.

## Features

The features used in the model include:

- `rolling_mean_temp`: Rolling mean of temperature readings.
- `vibration`: Vibration levels recorded by sensors.
- `acoustic`: Acoustic signals recorded by sensors.

The target variable is `failure`, indicating whether a wind turbine has failed.

## Modeling

A RandomForestClassifier is used for the classification task. The key steps include:

1. **Feature Engineering:** Extract relevant features and compute rolling statistics.
2. **Model Training:** Train the RandomForest model on historical sensor data.
3. **Evaluation:** Evaluate the model using precision, recall, and F1-score.

## Results

The model achieved the following performance on the dataset:

- **Precision:** 1.00 for both classes
- **Recall:** 1.00 for both classes
- **F1-Score:** 1.00 for both classes
- **Accuracy:** 1.00

The model predicts equipment failure with 100% accuracy on the given dataset.

## Usage

To use this project:

1. Clone the repository:
   ```bash
   git clone https://github.com/richardk100/predictive-maintenance.git
