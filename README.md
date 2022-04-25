# Flatiron - Capstone Project by Vi Bui
# DISCO DUO 
## Building Deep Nueral Networks using music data and Tensorflow to predict metrics such as danceability

<img src='Images/Disco Duo Logo Prototype.jpg'>

# Overview

**Client:** Existing or new music streaming services. Existing: Spotify, Pandora, Amazon Music, etc. New: companies interested in building new platforms to connect people through music. 

**Objective:** Create a platform where listeners of the same song are connected and able to discover new songs through their “connector song” by requesting another song based on a musical metric such as: danceability, loudness, acousticness, valence, etc.
 
**Data, Methodology, and Models** <br/> 

**Data source**: Spotify 
1. Spotify Song Data - https://www.kaggle.com/akiboy96/spotify-dataset
2. Spotify Genre Data - https://www.kaggle.com/code/akiboy96/spotify-song-popularity-genre-exploration/data?select=genre_music.csv

**Methodology:** Pull sample from data; create spectrogram images for songs; train model to predict danceability 

**Models:** Sequential Models 
1. Layers
2. Stochastic 
3. Add layers

**Target for first model: danceability** <br>
danceability: A value of 0.0 is least danceable and 1.0 is most danceable. Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity.

<br>

## BUSINESS VALUE
Connect people through music in a new way // connect people in a new way through music

<br> 

## OBSERVATIONS ABOUT THE DATA
Danceability is most strongly correlated with valence (happiness), popularity, loudness, and energy

<img src='Images/Song Metrics - Correlation Matrix.png'>

<br>

**Sample dataset had proportionately more Rock songs than the full dataset**

<img src='Images/Genre_Data.png'>

<br>

# Methodology 
## Spectrograms were used as images to model the data

<img src='Images/Spectrograms.png'>

# Models & Metrics 
## We ran three models and used RMSE (root mean square error), which tells us how close our models' predicted ratings are to actual danceability. 

<br>
While all models showed strong results and predictions, we chose Model 3, which had the best RMSE of of 0.0214, meaning our predictions, on average, were 0.0214 points away from actual danceability measure (range: 1-10). 

<br>

<img src='Images/Model3.png'>

<br>

 # **RESULTS & RECOMMENDATIONS** 

## Summary of recommendations

* All three Sequential Models performed well, and we feel most confident with Model 3
* With Model 3's RMSE (root mean squared error) = loss: 0.0214 - val_loss: 0.0183, our model shows it will be a strong predictor of "danceability" of songs 
* We will use the same approach in our Future Work with other metrics in the dataset 

<br>

## **FUTURE WORK**
* Run models for all remaining metrics: 
1. Energy
2. Speechiness
3. Acousticness
4. Instrumentalness
5. Liveness
6. Valence 
<br>
* Build platform to connect users listening to the same song and apply Disco Duo
<br>
* Expand ways to use Disco Duo (game night, silent discos, etc.)
<br>
**THANK YOU!!**

# Repository Structure

- Images 
- gitignore
- README.me
- Vi_Bui_Capstone_Presentation.key
- Vi_Bui_Capstone_Presentation.pdf
- Vi_Bui_Capstone_Submission_Jupyter Notebook.pdf
- Vi_Bui_Capstone_Submission.ipynb
- viiiiiiiiiii_Flatiron_Capstone_Final_Vi_Bui.pdf
