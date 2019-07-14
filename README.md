# NYC Taxi Trip Data Science Project

![picture alt](http://i.huffpost.com/gen/3118218/images/o-NEW-YORK-TAXI-facebook.jpg)


# Introduction
The New York City yellow taxi cabs are one of the most distinguishing symbols of the city that never sleeps. While there are numerous ways to get around the city, perhaps the most convenient way is via the taxi cabs. It gives people a chance to take a breather, sit back, relax, and use their phone for recreational or professional purposes. 

# Motivation
In a city that is always cluttered with millions of pedestrians, cars, public transit, and others, it would be beneficial to understand just how long you can expect your trip from point A to point B to take. Given various data about geolocation, trip duration, and the weather, it would be beneficial for both the taxi driver and the passengers to know when and where the taxi demand would be high, and also to know how long a trip can be expected to take. 

# Overview

The initial data cleaning/wrangling work can be found in the notebooks folder. The initial findings from the data analysis can also be found in the notebooks folder. 

The models folder contains several jupyter notebooks: 

1. Clustering notebook, which uses KMeans Clustering (with 15 clusters) to group the trips by their pickup location coordinates. These coordinate labels will later be used in other models as predictor variables. 
2. The ride duration prediction notebook, which uses both simple linear regression and XGBoost models. The scoring metric here will be judged by the Root Mean Log Squared Error, meaning that the predictions will be made on the log(trip_duration), and the scale will be in log-seconds.
3. Time Series Analysis notebook, which uses ARIMA and Seasonal ARIMA models to forecast taxi ride demand in NYC. 
4. Neural Network notebook, which contains both simple sequential neural networks and Long Short Term Memory (LSTM) network to forecast taxi ride demand in NYC.

# Findings

# Future Work
Other notable data can be wrangled to add more meaning or increase accuracy to the ride duration prediction models. An example might be finding data on if there were major events held in the city at some time (i.e at MSG or some other venue). This may very well cause traffic delays and jams. 
