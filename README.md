# flight_data

Flight data has the following features:

  arr_flights: Number of arriving flights

  arr_del15: Total number of delayed flights in observation

  carrier_ct: Total number of delays due to the carrier

  weather_ct: Total number of delays due to the weather

  security_ct: Total number of delays due to security. 

  on_time: Total number of on-time flights. 

Initially, I cleanse the dataset to predict if the delayed flight is "United" or not and run two Machine Learning models on it. 

The Confidence interval predicts the 95 percentile of the time of the delayed flights. 


**Please note that due to the limited size of the dataset, the Machine Learning models aren't compatible for other general models. While the accuracy, precision and recall is about perfect, it's because the test set only has limited data rows (unable to sample with replacement since there's high correlation between internal data values and creates overfiting/ underfitting issues.). One in theory could also run N sample with replacement on the dataset Y times (i.e. 1000) where N is less than the size of the dataframe and assess specific evaluation metrics to find the optimal N.**
