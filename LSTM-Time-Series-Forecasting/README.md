Objective of this project:
To predict the future values of the Bank Nifty index using different LSTM models and compare the performance of these models.
Then, based on metrics evaluation, decide the best-performing model. 
The performance evaluation metrics include Root Mean Squared Error (RMSE) and Mean Squared Error (MSE).  

The two main approaches considered so far:  
1. In the first approach, comparing the performance of different LSTM architectures, using the 
adjusted closing prices of the Bank Nifty index and its constituent banks as input. The model with 
the lowest root mean squared error (RMSE) is selected as the optimal architecture. 

2. The second approach builds upon the optimal architecture identified in the first approach, further 
enhancing the model by incorporating technical indicators (SMA, EMA, RSI, and MACD) in 
addition to the adjusted closing price as input features. The second approach further improves the 
performance as lower RMSE is achieved.
