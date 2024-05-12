# Air_quality_Forecasting
## Introduction
This project focuses on implementing a Long Short-Term Memory (LSTM) neural network for multivariate time series forecasting. The goal is to predict the PM2.5 concentration, a measure of air quality, using historical data on various environmental factors such as temperature, pressure, and wind speed. The project aims to provide insights into air pollution trends and assist in decision-making for environmental management.

## Key Steps
## Data Exploration and Preprocessing:

1. Load the dataset containing environmental variables and PM2.5 concentration.
2. Handle missing values and perform exploratory data analysis (EDA) to understand the data distribution and correlations.
3. Resample the data to a monthly frequency for better visualization and analysis.
4. Perform seasonal decomposition to identify patterns and trends in the data.
## Feature Engineering:

1. Create datetime features by combining year, month, day, and hour columns.
2. Drop unnecessary columns and set the datetime column as the index.
3. Perform one-hot encoding for categorical variables like wind direction.
## Normalization:
Scale the features using Min-Max scaling to ensure uniform ranges for model training.
## Create Sequences for LSTM Model:

1. Generate input sequences and target variables for training the LSTM model.
2. Define the sequence length (window size) and split the data into training and test sets.
   
## LSTM Model Development:

Build an LSTM model architecture using the Keras framework.
Configure the model with multiple LSTM layers followed by dense layers for regression.
Compile the model with appropriate loss function and optimizer.
Model Training and Evaluation:

Train the LSTM model using the training data and validate its performance.
Monitor training progress and apply early stopping to prevent overfitting.
Evaluate the model's performance using metrics such as Mean Absolute Error (MAE) and Root Mean Square Error (RMSE).
Results Analysis and Visualization:

## Visualize the predicted values against the actual values to assess model accuracy.
Calculate RMSE to quantify the model's prediction error.
Analyze the results to identify areas of improvement and potential insights.
Forecasting:

Utilize the trained LSTM model to forecast PM2.5 concentration for future time steps.
Update input sequences with forecasted values for iterative forecasting.
![](https://github.com/cleavestone/Air_quality_Forecasting/blob/main/forecast.png)
