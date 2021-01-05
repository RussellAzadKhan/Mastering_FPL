# Mastering_FPL

## Statistical analysis and predictive modelling of Fantasy Premier League data

Fantasy Premier League (FPL) is an online game where you choose your own team of Premier League footballers. If your players do well in real life games, you get points. It's that simple. 

The aim of this project is to see if current data science methods are able to predict the performance of Premier League Players to a level which would be useful for FPL team selection. 

The dataset for this project has been forked from Github user Vaastav (https://github.com/vaastav/Fantasy-Premier-League). The dataset spans 4 seasons: 16-17, 17-18, 18-19, 19-20. The dataset contains player performance data (points, goals, assists etc.), as well as numerous metrics related to player performance (cost, threat, creativity, etc.). 

Other notable projects I have come across are Github user solpaul (https://github.com/solpaul/fpl-prediction) who looked at weekly player forecasts. As well as from Github user nuebar (https://github.com/nuebar/forecasting-fantasy-football) who built a model to optimise team selection. 

Influenced by these projects, the hypothesis I first wanted to test was whether player performance for a whole season (FPL points total), could be predicted based on the previous season. Using a random forest regression model an adjusted r^2 of 0.43 was achieved. 

I then decided to simplify the problem into predicting whether a player will improve on their previous season. This is an example of a classification problem. Using Kernel SVM an accuracy on 62% was achieved. 
Using K-means clustering I was able to identify 4 clusters of FPL players based on their cost, and total points for a season: 
(1) Low cost, low points 
(2) Low cost, high points 
(3) High cost, low points 
(4) High cost, high points 

Using TensorFlow to create a deep neural net I was then able to predict with 56% accuracy the cluster that a player would be in.

This project is still a work in progress.
