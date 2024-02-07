# Time series analysis and visualization
This exercise in TS analysis is a logical evolution from the very first attempt to predict anything based on the historical time-series data found in /stock_prediction repo. 

A number of approaches will be evaluated and tested. 

## Comparison of Time Series, Machine Learning, and Deep Learning models

Various models will be explored to forecast Adjusted Close prices for HSBC stock price data from simple machine learning algorithms such as Moving Average, Linear Regression and k-Nearest Neighbours, to Auto ARIMA, Facebook's Prophet, and LSTM.

## Time Series and Forecasting Models: ARIMA

There are many ways to model a time series in order to make predictions including Moving Averages MA(q), Autoregression AR(p), and combining these to create ARMA(p,q), ARIMA(p,q,d), SARIMA(p,q,d)(P,Q, D,s) models.

An attempt to build, test, and validate an AutoRegressive Integrated Moving Average (ARIMA) model will be made.

## Time Series and Forecasting Models: SARIMA

The Seasonal Autoregressive Integrated Moving Average (SARIMA) model combines simpler models to capture moving averages throughout time series, taking into account trend, seasonality, and noise.

An attempt to build, train, and test a SARIMA model for predicting HSBC Adjusted Close price patterns will be made.

## Regression Models

Ten years of HSBC Adjusted Close price historical data will be used to see if it is possible to forecast out 'n' days in the future. Several models will be compared to see whether Gradient-descent-based, Distance-Based, or Tree-Based algorithms perform best.

After a backtest of the models, the best performing will be selected and Grid Search cross-validation will then be used to find the best parameters for tuning the models, as well as visualizing the results.

## Classifier Models

Predicting the direction of stock prices allows the analyst to classify stocks as Buy if the price will increase 'n' days in the future, or Sell if it will decrease.

An attempt to create a pipeline of several classifier models will be made to streamline the selection process. After the validation of the models, the top three will be selected based on evaluation metrics in the classification report. Grid Search across validation will then be used to find the best parameters for tuning the models, and confusion matrices will be plotted to better visualize performance.

## Deep Learning: LSTM

A separate attempt in Long Short-Term Memory. Five years' worth of HSBC historical data will be used to predict Adjusted Close prices by building a multi-layer LSTM Recurrent Neural Network model. The ability to store information over some time is useful when dealing with time series data.

## Deep Learning: RNN, LSTM and GRU

A simple Recursive Neural Network model will be trained on HSBC stock data followed by Long Short-Term Memory and Gated Recurrent Unit models which were developed to overcome the vanishing gradient problem. Results will be compared.

## TS and Forecasting Models: FB Prophet

Prophet (an open-source lib built upon scikit-learn) automatically detects changes in trends by selecting changepoints from the data. It is an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, as well as holiday effects, and includes automatic detection for all values.
