# Time-Series-And-Anomaly-Detection
In this repository, I have used ARIMA,SARIMA,AutoArima,ANN,CNN and LSTMs for time series modelling and Anomaly detection has been done using LSTM+Autoencoders.
## References
1) **Analytics Vidhya Article on ARIMA and Autoarima**:-(https://www.analyticsvidhya.com/blog/2018/08/auto-arima-time-series-modeling-python-r/) 
2) **Geeks For Geeks article**:- (https://www.geeksforgeeks.org/python-arima-model-for-time-series-forecasting/)
3) **Johnson and Johnson Stock Price Anomaly Detection**:-(https://morioh.com/p/ab2d9412ff57)
### About Dataset 
In this repository I have used 2 different datasets, one of johnson and john stock prices for anomaly detection which has been uploaded and second of US Airline Passengers for time series analysis from Kaggle.The dataset has been imported from Kaggle with the following link:- 
https://www.kaggle.com/chirag19/air-passengers/download
<br>
<br>
The Time Series had to made **stationary**. This was done using **differencing operation** and **exponentially weighted averages**.The Time Series was analysed using **ARIMA** and later **seasonal ARIMA(SARIMA)** since normal ARIMA was unable to give good predictions. Hence SARIMA proved to be awesome. Implememntation of **AutoArima** has also been displayed which doesn't require any differencing to make series stationary or draw **acf and pacf plots** in order to determine values of order of lags of MA(p) and AR(q).
<br>
The above Time Series Model has also been analysed using Deep learning Techniques like Artificial Neural Networks, Convolutional Neural Networks and LSTMs and the predcitions were 
plotted with the actual values.
<br>
**Anomaly Detection** has been implemented on **Johnson and Johnson Stock Prices** Dataset which was updated from **4 September 1985** till **3 September 2020** using LSTM+AutoEncoders. LSTMs were employed because they are good with understanding sequential data while the purpose of Autoencoders is just dimensionality reduction,i.e- it has to learn the representation of our dataset and understand which range of errors between actual and predicted values is acceptable. If an error falls above that threshold I would classify it as an anomaly. In the dataset the anomaly was observed for the months of March and April 2020.
