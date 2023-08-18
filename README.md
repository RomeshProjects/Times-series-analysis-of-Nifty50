# Times-series-analysis-of-Nifty50

For our self-project involving time series analysis and stock price prediction, we followed these steps and used various techniques:

Data Selection and Preparation:

We selected the Nifty-50 indices and Microsoft stock price as our datasets.
We performed Augmented Dickey-Fuller (ADF) tests to determine the stationarity of the time series data, as stationarity is crucial for many time series analysis methods.
Seasonal Decomposition and Data Differencing:

We applied seasonal decomposition to break down the time series data into trend, seasonal, and residual components.
We utilized data differencing techniques to transform the data and make it more stationary, helping to eliminate trends and seasonality.
Exponential Weighted Moving Average (EWMA):

We employed the Exponential Weighted Moving Average (EWMA) technique to estimate the underlying trend by giving more weight to recent observations. This helps reduce the impact of older data on predictions.
ARIMA Modeling:

We implemented the AutoRegressive Integrated Moving Average (ARIMA) model, which combines autoregressive (AR) and moving average (MA) components.
The ARIMA model yielded an MSE (Mean Squared Error) of 18%, indicating the average squared difference between predicted and actual values. A lower MSE signifies better model performance.
SARIMAX Modeling:

We extended the ARIMA model with seasonal components using the Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors (SARIMAX) model.
Although we didn't specify the performance metric for SARIMAX, it's a suitable choice for datasets with noticeable seasonal patterns.
LSTM Modeling:

We experimented with Long Short-Term Memory (LSTM), a type of recurrent neural network (RNN) well-suited for capturing long-range dependencies in time series data.
Our LSTM model achieved an MSE of 10%, showcasing its ability to capture complex patterns in the data.
Evaluation:

We employed the Mean Squared Error (MSE) as the performance metric for both the ARIMA and LSTM models. A lower MSE indicates higher predictive accuracy
