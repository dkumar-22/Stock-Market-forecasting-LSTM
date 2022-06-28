# Stock-Market-forecasting-LSTM
Stock Market Forecasting using Long Short Term Memory. The Dataset Used was for Apple. An LSTM model based on their historical Stock Prices was built which was able to predict and forecast the stock prices for the next 30 days after the Dataset end date.

<center>
<img src="https://miro.medium.com/max/1400/1*-LxiGnfFs_7oQ7c0ErvmWQ.png" alt="lstmImg"/>
</center>

Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) architecture.
LSTM networks are well-suited to classifying, processing and making predictions based on time series data, since there can be lags of unknown duration between important events in a time series. LSTMs were developed to deal with the vanishing gradient problem that can be encountered when training traditional RNNs. There are three different gates in an LSTM cell: a forget gate, an input gate, and an output gate. Relative insensitivity to gap length due to these gates solves the long-term dependency problem is an advantage of LSTM over RNNs, hidden Markov models and other sequence learning methods in numerous applications.

## Working

It works on the Dataset as shown, it is a .csv file that contains 1258 records each corresponding to the various information related to stocks of a company (Apple in this case) for a particular day. 
We will be predicting the Stock Prices using the close price on a day using LSTMs.
With the help of LSTMs we train the model such that it studies the close prices for 100 days, with the help of the trends observed the model predicts the close price for the 101th day.

<br/>
We make predictions for the close prices of the stock. We divide the data into training set and test set. With 65% of the data used for training while the rest is used for predictions. We then calculate various error metric to see how our model performs.
