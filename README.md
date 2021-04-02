# Predicting Artist Genres

Authors: Donna Lee & Jake Ash

## Overview 

Using a dataset (https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks) from Spotify, we looked at genre by artists from the years 1921 to 2021. The dataset included mean attributes (listed below) of all the artist's songs and their genre tags. 

We noticed that around 58% of the artists did not have any genre tags so we wanted to create a prediction model to predict the general genre of the artist. 

Attributes
* Acousticness
* Danceability
* Duration 
* Energy
* Instrumentalness
* Liveness
* Loudness
* Speechiness
* Tempo
* Key
* Mode
* Count

## EDA




## Model Selection and Tuning

We ran three models - KNN, Random Forest and XGBoost and optimized towards a F1 Score. Precision and recall were equally important to us. 

    Model     | F1 Score
------------- | -------------
Random Forest |   0.8226
     KNN      |   0.6548
   XGBoost    |   0.8182

## Predictions 
