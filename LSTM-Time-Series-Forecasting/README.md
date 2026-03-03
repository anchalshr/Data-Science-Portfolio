## Objective of this project:
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

## Dataset
Data for the 12 constituent stocks of the Bank Nifty index is fetched using the yahoofinance library, 
covering the period from January 1, 2019, to April 1, 2024. A dataset is created for the Bank Nifty 
index and its 12 constituent banks, incorporating various technical indicators such as SMA (Simple 
Moving Average), EMA (Exponential Moving Average), RSI (Relative Strength Index), and MACD 
(Moving Average Convergence Divergence). 

## Methodology
The study is divided into several phases: 
1. Optimizing the LSTM architecture. 
2. Testing different dataset preparation techniques 
3. Evaluating the effects of various inputs, such as adjusted closing prices and technical indicators, 
on prediction performance.

## Results
The best-performing model configuration included a stacked LSTM structure, which minimized 
prediction error with an RMSE of 2084.37, using Adam as the optimizer, ReLU activation, and 
Dropout regularization.  


