# Project Overview
In this project, we'll predict the winner of football matches in the English Premier League (EPL).
The main goal is to predict whether a team wins a game or not. So, loses and draws will be combined and given the same encoding.

**Project Steps**
* Scrape match data using requests, BeautifulSoup, and pandas.  
* Clean the data and get it ready for machine learning using pandas.
* Make predictions about who will win a match using scikit-learn.

## Data
* We'll be scraping [FBref](https://fbref.com/en/) to get our data.
* Specifically, we collect match data from the 2017 to 2024 seasons for training and testing the model

## Model
* We used 55 features, including metrics such as xG (expected goals), xA (expected assists), GA (goals against), GF (goals for), and others for each Premier League team to train our model.
* A Random Forest Classifier with 50 decision trees was used to power the predictions.
* Weights are given to different seasons to train our model effectively. The older seasons were given lower weights and the recent seasons were given a higher weight.

## Results
The model achieved 68.1% accuracy, measured using precision, F1 score, and recall.
