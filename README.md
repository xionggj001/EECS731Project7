# EECS731Project7
The Oscars

The data is the 'Beijing_housing_price.csv', which is chosen from the semester project.

In this project, we first analysis the data by finding the distribution of each features and calculate the correlation between any two features. We also demonstrate the housing price over time.  Base on the analysis, we aim at predicting the house price for given features and forecasting the trend for the housing price in Beijing. 

There are features ['Lng', 'Lat', 'tradeTime', 'DOM', 'followers', 'totalPrice', 'price',
       'square', 'livingRoom', 'drawingRoom', 'kitchen', 'bathRoom',
       'buildingType', 'renovationCondition', 'buildingStructure',
       'ladderRatio', 'elevator', 'fiveYearsProperty', 'subway', 'district',
       'communityAverage'] in this data set. 
 However, for training purpose, we won't use all of them. We only select parts of them to reduce traing overhead and improving the performance as well. The choosing criterion is based on the correlation we characterized.
 

# Part 1: Prediction 

This part aims at predict the exact housing price with particular feathers. We adopt the following three models:

Model 1: Linear Regression
Model 2: Linear SVM
Model 3: Neural Network

The original data sets were divided into training and testing data set with the ratio of 80% and 20%. All the regressors demenstrate high accuracy for prediction and among them, NN is the best due to nonlinear property.




# Part 2: Time Series Forecasting

Thia part aims at predicting the trend of housing price for Beijing and KC. We transform the data sets into the time series data frame and characterize the trend of housing price for the given data sets.  The housing price in Beijing has the potential to grow in the near future, while the trend of that of KC will keep stationary for a long period.

Two models are adopted for the time series forecasting: 

Model 1: ARIMA
Model 2: Prophet 

For Beijing housing price data, both models can predict the increasing trend in the future, while the Prophet can outperform ARIMA in the sense of actual housing price.

