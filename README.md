# 16_AzkaDalvi_Assignment1

# Student Assignment Details
This project is submitted as part of the DAV assignment, by Azka Dalvi.
The assigned publicly traded stock for analysis is ASIANPAINT.

# Objective
The objective of this project is to analyse the daily closing prices of ASIANPAINT using historical stock market data from the NSE website and apply the ARIMA model for time series forecasting.
The project includes data preprocessing, stationarity testing, ARIMA model implementation, and forecasting of the next 30 days' closing prices.

# Dataset Information
- Stock Name: ASIANPAINT
- Stock Exchange: NSE (National Stock Exchange)
- Dataset Type: Daily Historical Data
- Time Period: Past 1 year
- Source: NSE Historical Data

# Project Tasks Performed
1. Data Preprocessing

The following preprocessing steps were performed on the dataset:

- Converted the DATE column into proper datetime format
- Cleaned numeric columns by removing commas and converting to numeric values
- Checked and handled missing values
- Sorted the dataset in chronological order
- Set the DATE column as the index
- Visualized the closing price trend over time

2. ARIMA Model Implementation

The following steps were used for ARIMA modeling:

- Conducted the ADF (Augmented Dickey-Fuller) Test to check stationarity
- Applied first differencing to make the series stationary
- Used ACF and PACF plots to determine initial ARIMA parameters
- Evaluated multiple models using AIC (Akaike Information Criterion)
- Selected ARIMA(2,1,1) as the optimal model
- Fitted the model to the time series data
- Performed residual analysis to validate model performance

3. Future Price Prediction

The trained ARIMA model was used to:

- Forecast the next 30 days of closing prices
- Visualize forecasted values along with historical data

# Libraries Used
The following Python libraries were used in this project:

- pandas
- numpy
- matplotlib
- statsmodels
- scikit-learn

# Files Included in the Repository
AI_Ethics_Declaration_Page.docx - Ethics Declaration
DAV_Assignment_1.ipynb - Source Code
Quote-Equity-ASIANPAINT-EQ-19-04-2025-19-04-2026.csv - Dataset
README.md - Project Documentation

# Results and Observations
The following observations were made:

- The stock prices showed fluctuations over the observed period
- The time series was initially non-stationary and was made stationary using differencing
- ACF and PACF plots suggested an initial ARIMA model, which was refined using AIC
- ARIMA(2,1,1) provided the best fit based on AIC comparison
- Residual analysis indicated that the model errors resemble white noise
- The forecasted values show short-term stability with minor fluctuations

# Conclusion
This project demonstrates the application of the ARIMA model for time series forecasting of stock prices.
Using historical data of ASIANPAINT, the model was trained and used to predict future values. The results suggest a relatively stable trend in the short term, though actual prices may vary due to external market factors.

# AI Ethics and Responsible Usage Declaration
This project is developed strictly for academic and educational purposes only.

- Forecasts are based only on historical data and statistical modeling
- Results should not be used for financial or investment decisions
- Only publicly available NSE data has been used
- No private or restricted data has been included
- The project follows responsible and ethical data usage practices

# Academic Integrity Declaration
I declare that this work is my original submission for academic purposes.
All references and resources have been acknowledged where applicable.
No plagiarism has been intentionally committed.

# How to Run the Project
In Google Colab
1. Open the notebook file
2. Upload the dataset file ASIANPAINT.csv
3. Run all cells sequentially
4. View graphs and forecast results
5. Download outputs if required
