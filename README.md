# Final Project: Spotify Song Genre Prediction

UC Berkeley MIDS Program 

Shuo Wang, Ivan Escalona, Daisy Khamphakdy, Iris Lew, Amanda Teschko

December 2022

- [Final Project: Spotify Song Genre Prediction](#final-project-Spotify-Song-Genre-Prediction)
  - [Project Overview](#project-overview)
  - [Dataset](#dataset)
  - [EDA](#EDA)
  - [Feature Engineering](#Feature-Engineering)
  - [Models](#Models)
  - [Results and Discussion](#Results-and-Discussion)
  - [Helpful Information](#helpful-information)
    - [Environment](#environment)

## Project Overview
This project is to build machine learning learning models to have the music app automatically recognize a song’s genre when a song is added to its database, rather than manually classifying a song genre. 

## Dataset
Kaggle link: https://www.kaggle.com/datasets/mrmorj/dataset-of-songs-in-spotify

Dimension: 42,305 rows x 22 columns

Features: 
‘danceability', 'energy', 'key', 'loudness', 'mode', 'speechiness', 'acousticness', 'instrumentalness', 'liveness', 'valence', 'tempo', 'type', 'id', 'uri', 'track_href', 'analysis_url', 'duration_ms', 'time_signature', 'genre', 'song_name', 'Unnamed: 0', 'title'

Data dictionary:
https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features

https://docs.google.com/document/d/1LWl88F8wGY1WkkOSzzVzwSYij1yeMR8hFXllRpkMyrI/edit

## EDA 
- Underground rap was the most popular genre
- Imbalance in the records per genre
- Some numeric features are on different scales
- Some fields has high levels of missing data
- Some rows are duplicated
- Some tracks are mapped to more than one genre

![alt text](https://github.com/Shuo-Wang-UCBerkeley/2022-fall-assignment-W207-Spotify-Song-Genre-Prediction-Final_Project/blob/main/Images/EDA.png)

![alt text](https://github.com/Shuo-Wang-UCBerkeley/2022-fall-assignment-W207-Spotify-Song-Genre-Prediction-Final_Project/blob/main/Images/Addressing_Imbalanced_Data.png)

## Feature Engineering
![alt text](https://github.com/Shuo-Wang-UCBerkeley/2022-fall-assignment-W207-Spotify-Song-Genre-Prediction-Final_Project/blob/main/Images/Feature_Engineering.png)

## Models
- Baseline Models: **ALWAYS** predict the most most popular genre from the raw data (Underground Rap)
- Random Forest
- XGBoost
- Neural Networks
- K-Means
- K-Nearest Neighbors
- Logistic Regres

## Results and Discussion
- Feature scaling and balancing data is crucial for some models
- The benefits of different feature engineering techniques will vary from model to model
- Establishing a baseline gave us better appreciation for our model, even though the accuracy wasn’t objectively high
- More investigation into balancing techniques could be helpful

![alt text](https://github.com/Shuo-Wang-UCBerkeley/2022-fall-assignment-W207-Spotify-Song-Genre-Prediction-Final_Project/blob/main/Images/Results.png)

## Helpful Information
### Environment
Google Colaboratory

[Back-To-Top](#final-project-Spotify-Song-Genre-Prediction)