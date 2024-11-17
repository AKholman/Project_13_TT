Data Projects (TripleTen)
# Project_13_TT
Project_13  Time Series Analysis:
Project-13: Time Series Forecasting of Taxi Orders for Peak Hour Prediction

## Project Overview

**Sweet Lift Taxi Company** has gathered historical taxi order data from airports to optimize driver allocation during peak hours. The company needs to predict the number of taxi orders for the next hour to improve efficiency in driver distribution. The objective of this project is to analyze and forecast taxi orders using time series models, with the goal of accurately predicting demand during peak times.

This project focuses on using various time series models to forecast the number of taxi orders for the upcoming hour, ensuring that the Root Mean Squared Error (RMSE) metric on the test set does not exceed 48.

## Project Description

To forecast taxi orders, the dataset was resampled to hourly intervals and analyzed for trends, seasonality, and residuals. The following steps were taken:

1. **Data Preprocessing**: The dataset was resampled to an hourly frequency to standardize the data and fill any gaps or inconsistencies.
   
2. **Time Series Decomposition**: We decomposed the time series into its components: **trend**, **seasonality**, and **residuals** to gain insights into the patterns underlying the data.

3. **Modeling**: We implemented and evaluated multiple time series models to forecast taxi orders. These models included:
   - **Autoregressive (AR) Model**
   - **Autoregressive (AR) Model with Hyperparameter Optimization**
   - **Moving Average (MA) Model**
   - **ARMA Model**

4. **Model Evaluation**: The performance of each model was evaluated using **Root Mean Squared Error (RMSE)**. All models were optimized to ensure that the RMSE on the test set did not exceed the threshold of 48.

## Data Description

The dataset `taxi.csv` contains historical taxi order data with the following columns:

- **num_orders**: The number of taxi orders for a given time period.
- The data has been resampled to a one-hour frequency, ensuring that each record corresponds to a specific hour of taxi order data.

You can find the dataset in the `taxi.csv` file. Ensure you have this file available to run the analysis.

## Requirements

To run this project, you will need the following Python libraries:

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **matplotlib**: For visualizations.
- **statsmodels**: For time series analysis and modeling.
- **pmdarima**: For Auto ARIMA model selection.

You can install the required libraries by running:

pip install pandas numpy matplotlib statsmodels pmdarima


Conclusion
The project successfully utilized various time series forecasting models to predict the number of taxi orders at airports, with the aim of optimizing driver allocation during peak hours. By applying Autoregressive (AR), Moving Average (MA), and ARMA models, we were able to achieve accurate forecasts, with RMSE values consistently below the threshold of 48.

Key Findings:
Autoregressive (AR) Model: Achieved accurate predictions based on the autocorrelation patterns.
Hyperparameter-Optimized AR: Improved model performance by fine-tuning hyperparameters.
Moving Average (MA) Model: Performed well in capturing short-term dependencies.
ARMA Model: The most flexible model, combining both AR and MA components, providing strong results.
All models were able to predict taxi orders with high accuracy, allowing the Sweet Lift Taxi company to optimize driver allocation during peak hours.

