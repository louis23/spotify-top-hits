# Hit or Miss: Predicting the Success of Songs on the Spotify Leaderboard

## Problem Statement: Every song, regardless of genre, old or new, has audio features like acousticness, danceability, tempo etc. What kind of audio features do popular songs have? Do Spotify hits or Billboard Top 100 have similar sound signatures? This project will seek to find out.
## Deliverable: A classification model which predicts if a song will make it to the top 100 (or not), based on its audio features.

The aim is to develop a classification model which predicts if a song will make it to the top 100 (or not), based on its audio features.
This project was done with my classmate Nate Ng who has also featured this project on his Medium (https://medium.com/@nthnil)

## Web Deployment: https://spotifypredapp-cvmugwf2pxpmrztam4z2yn.streamlit.app/

1. Type in the name of the song you want to predict
![Deploy_1](https://github.com/user-attachments/assets/9e1eea72-c17d-42fb-b08d-30c15b81adc6)

2. Select the correct song if there are multiples with the same name
![Deploy_2](https://github.com/user-attachments/assets/0102fd62-c0b2-4c48-b404-fa723b4246a2)

3. Our model will tell you if it thinks this song will be a hit!
![Deploy_3](https://github.com/user-attachments/assets/e9e440df-5112-4c8c-9983-42c0f1674b08)


Data collected:
- 5000 songs (not in top 100, from Kaggle)
- 1000 songs (top 100 from past 10 years, from Spotify api)

Machine learning models experimented:
- SVM
- Decision tree
- K-NN
- Logistic regression
- Adaboost
- XGBoost

## Feature Importance
### Final Audio Feature Set
● Danceability
● Energy
● Linear Loudness
● Speechiness
● Acousticness
● Instrumentalness
● Liveness
● Tempo
● Valence
● Duration (ms)

Our best performing model was the hard voting classifier with random forest, adaBoost and XGBoost as the base estimators.

Evaluation metric used:
- F1 score (combination of precision and recall, imbalanced dataset)
- ROC-AUC (higher is better)

![Screenshot 2025-06-08 at 6 26 45 PM](https://github.com/user-attachments/assets/dd4c04f5-ff81-48dd-8c38-693c9d907b35)

![Screenshot 2025-06-08 at 6 26 59 PM](https://github.com/user-attachments/assets/704eba57-bc2e-4a71-b5c3-e5f691b88aae)

## Areas for improvement

![Screenshot 2025-06-08 at 6 30 27 PM](https://github.com/user-attachments/assets/93ef63eb-e1a9-45f1-bd72-25318fd51688)


