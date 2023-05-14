# Stock_Prediction.Linear.Reg

a)downloaded the historical price data for the Apple Inc., Amazon, Netflix and Tesla using the yfinance library,
from the start of 2010 to May 14, 2023.

b)Scaled the closing prices using MinMaxScaler to constrain the values between 0 and 1.

c)Defined a function create_dataset that transforms the time series data into a format suitable for supervised learning. The function takes
  two arguments: 1.The dataset (NumPy array that we want to convert into a dataset)  
                 2.look_back (which is the number of previous time steps to use as input variables to predict the next time period)
d)  We then use this function to reshape our data into the format: [sample, features].

e)  split the prepared dataset into training and testing datasets, using 80% of the data for training and the remaining 20% for testing our model.


f) Finally, created a Linear Regression model and training it on our training data (X_train and Y_train).

g) Used the trained model to make predictions on our testing data (X_test).

h) Evaluated the performance of our model by calculating the Root Mean Squared Error (RMSE). The RMSE is a measure of how well the
   model performed. It does this by measuring the difference between the predictions of the model and the actual values. 
   
i) denormalized our predictions. This is because we transformed our data to fit between 0 and 1 for our model, but we
   want to interpret the predictions in the original scale.
   
j) Finally, plotted predicted and original values of the stock prices.

    

