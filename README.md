# ForecastingProject1

In this project I will be forecasting U.S. inflation over a 12-month period. I will start with the Stock and Watson (1999) equation for determining inflation. This model revolves around the conventional Philips curve using unemployment and price level. I will be using a training sample from January 1982 to December 2018 and measuring my forecast against actual data from January 2019 to the most recently available data. All data will be retrieved from the Federal Reserve Economic Database in St. Louis.

The data I will be using: Personal Consumption Expenditures price index, chained to 2012, seasonally adjusted, measured in percent. We also will be using monthly seasonally adjusted Unemployment Rate, measured in percent. Non-seasonally adjusted one-year expected inflation rate, measured in percent. Seasonally adjusted total capacity utilization per month, measured in precents. Seasonally adjusted new privately-owned housing units starts, measured in thousands of units per month.

The data I gathered from FRED is not stationary data, non-stationary data makes effective time series analysis practically impossible. Non-stationary time series data will have a systematic change that are unpredictable.

I will be using the KPSS unit root test to test for the number of unit roots I have in each variable. Unit root tests will tell me if our data is stationary or not. For variables that I find to have a unit root, I will be transforming those variables accordingly converting them to stationary data.

I will be using a basic Time Series Linear Models from the FPP3 package in R-studio.

I then use the Mean Absolute Percentage Error (MAPE) for the accuracy measure of each forecast. I then use residual testing to check for autocorrelation and heteroskedasticity. 

I then create an ensemble model using all four variable's to forecast inflation. 

I found that the ensemble mode produces the most accurate forecast compared to the others, however, a simple Time Series Linear Equation leaves much to be desired. Trying to forecast inflation is difficult, however, this analysis is a good start.
