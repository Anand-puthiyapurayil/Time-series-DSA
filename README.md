# Time-series-DSA

For the practical work, we have used the Pump Sensor dataset that can be downloaded from here:
https://www.kaggle.com/datasets/nphantawee/pump-sensor-data

This dataset consists of 51 numerical features and a categorical label. 
•	51 numerical features contain raw sensor readings from 51 different sensors that are used to do condition monitoring of the pump.
•	The label contains string values that represent normal, broken and recovering operational conditions of the pump. The data set represents 219,521 readings from 51 sensors.
We are detecting anomalies with the given labels for Broken and Recovering. 

Solution Approach:
We have first built a model using MAD (mean absolute deviation) technique, we have imported the model from Pyod Library and then we have implemented two more unsupervised learning algorithms i.e., Naïve approach and VAR to compare their performances and accuracies. For doing so, we have followed the following steps:
•	Data source loading – We read the data from csv files. 
•	Data wrangling
•	Exploratory Data Analysis (EDA)
•	Pre-Processing
•	Feature Selection – For feature selection we classified the data using a Random Forest Decision Tree and got best performing sensors.
•	Modelling and Model Evaluation – We evaluated the models by considering F1 score.

Techniques Used 
-MAD (mean absolute deviation) of a data set is the average distance between each data value and the mean. Mean absolute deviation is a way to describe variation in a data set. Mean absolute deviation helps us get a sense of how "spread out" the values in a data set are.
-Naive approach using global mean and standard deviation
-VAR model extends the univariate autoregressive (AR) model by capturing the linear relations between multiple variables. For each input series, a regression is carried out. The original variables are regressed against their own lagged values and the lagged values of other variables. 

