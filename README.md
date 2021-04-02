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

For our initial model, we chose four distinct general genres (Rap, Jazz, Classical, and Country) to map the genres to. 

![image](https://user-images.githubusercontent.com/76017120/113424460-32b87f80-939e-11eb-9127-c2601a1441ed.png)

* All four genres had similar levels of artist counts so class imbalance was not a big concern. The four genres all had a little over 1,000 artists. 

![image](https://user-images.githubusercontent.com/76017120/113427946-eec87900-93a3-11eb-8034-b159700d56aa.png)

Some important features in predicting genres: 
* Acousticness
* Instrumentalness
* Duration (Seconds)
* Key of 7


## Model Selection and Tuning

We ran three models - _KNN_, _Random Forest_ and _XGBoost_ and optimized towards a F1 Score. Precision and recall were equally important to us. 


| Model         | F1 Score    |
| -----------   | ----------- |
| Random Forest |   0.8226    |
|  KNN          |   0.6548    |
|  XGBoost      |   0.8182    |

Our **Random Forest** model had the highest F1 score so we decided to use that to predict the missing genres of our artists.

![image (2)](https://user-images.githubusercontent.com/76017120/113428234-6eeede80-93a4-11eb-8ba5-844b29d0e14e.png)

Based on the confusion matrix, our random forest model had limited number of wrong predictions. This model was especially good at predicting classical music.


## Predictions 






