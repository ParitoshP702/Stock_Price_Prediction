# Stock_Price_Prediction
Predicting the price of stocks using neural network architecture through tensorflow
In this project I have used the dataset from kaggle:(kaggle datasets download -d andrewmvd/sp-500-stocks) which contains the data of the 500 stocks of the Standard and Poor's 500(The most famous financial benchmark in the world). I have used the data of MMM stocks , specifically the Adjusted Closing price of the stocks(3210 datasets to be specific) to predict the price of the stocks in the pseudo future horizon.
To predict the stock prices I have used the neural network architecture in tensorflow.
Firstly, I preprocessed the data in the framework of windows and horizons (window size = 7 and horizon = 1) and the split the data into training and test sets.
Then I made our first model consisting of dense layers to predict the stock price , I have also use a model checkpoint callback in order to save the model with best validation accuracy and validation loss.
After this I tried to predict the stock prices on our best model obtained through the model checkpoint callback.
Then I made our second model using one dimensional Convolutional Neural Networks (which are used widely on data based on sequence models) and did the same for this model.
After this I made an LSTM(Long Short Term Memory ) model using transfer learning approach with the Functiuonal API.
Lastly I have created a function to calculate all the evaluation metrics(namely, MAE, MSE, MAPE, MASE) and fed our 3 different models in that function to compare their results.
In the end I also visualised the models graphically by plotting them.
