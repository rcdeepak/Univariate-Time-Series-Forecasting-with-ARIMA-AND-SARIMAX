
# Univariate Time Series Forecasting using ARIMA AND SARIMAX

Time series forecasting is one of the most important topics in data science. Almost every business needs to predict the future in order to make better decisions and allocate resources more effectively.

This project focuses on utilizing ARIMA (AutoRegressive Integrated Moving Average) and SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous factors) models to forecast monthly Champagne sales for the next two years. The dataset used for analysis is the "Perrin Freres Monthly Champagne Sales" dataset sourced from Kaggle.


## Objective
The main objective of this project is to accurately predict Champagne sales for the upcoming two years based on historical sales data. By employing time series analysis techniques and the ARIMA and SARIMAX models, we aim to capture and account for the underlying patterns and seasonality in the data, resulting in reliable sales forecasts.
## Dataset Used
The dataset used in this project is the "Perrin Freres Monthly Champagne Sales" dataset obtained from Kaggle. It comprises monthly sales data of Champagne from Perrin Freres over a specific time period. The dataset contains the following columns:

 Date: Monthly time stamps

 Sales: Champagne sales in units
## Prerequisites
To run the project code and reproduce the results, the following libraries and dependencies need to be installed:

Python (version 3.9)

pandas 

numpy 

matplotlib 

statsmodels 

scikit-learn 

## Methodology
1. Data Preprocessing:
-   Importing the necessary libraries
-   Loading the Champagne sales dataset
-   Cleaning the dataset by handling null values, ensuring proper date format, and setting the index to the month column
-   Visualizing the sales column to gain insights into the data
2.  Seasonal Decomposition:
-   Utilizing the seasonal decomposition function from the statsmodels library to analyze the trend, seasonality, and residual components of the data
-   Plotting the trend, seasonal, and residual graphs
3.  Stationarity Check:
-   Conducting the Augmented Dickey-Fuller (ADF) test to assess the stationarity of the data
-   Observing the p-value to determine stationarity
4.  Data Transformation:
-   Implementing the rolling mean difference to make the data stationary
-   Verifying stationarity after the transformation
5.  Model Building and Forecasting:
-   Importing the ARIMA model
-   Fitting the data to the ARIMA model
-   Evaluating the model using the Akaike Information Criterion (AIC) score
-   Assessing the forecasted values against the actual data
-   Improving Seasonal Forecasting with SARIMAX:
-   Importing the SARIMAX model
-   Fitting the data to the SARIMAX model
-   Comparing the AIC score with the ARIMA model for evaluation
-   Plotting the forecasted and actual values to visualize the model's accuracy
7.  Result Analysis:
-   Computing the Root Mean Squared Error (RMSE) value to assess the performance of the forecasts
-   Forecasting the Champagne sales for the next two years based on the SARIMAX model
## Results
The SARIMAX model outperformed the ARIMA model in terms of forecasting accuracy, yielding a lower AIC score. The forecasts obtained from the SARIMAX model closely matched the actual sales data, demonstrating the model's ability to capture and account for the underlying seasonality in the Champagne sales dataset. The computed RMSE value of 240 indicated