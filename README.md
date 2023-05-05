# Project-2

## Problem:
I want to accurately predict the winners of NBA games. This is important to teams as well as betting companies to determine if their team has a good chance of winning.

## [Data source](https://www.kaggle.com/datasets/nathanlauga/nba-games?resource=download&select=games.csv)

## Description
This dataset was collected to work on NBA games data. Uses nba stats website to create this dataset.

There are 5 datasets :
- games.csv : all games from 2004 season to last update with the date, teams and some details like number of points, etc.
- games_details.csv : details of games dataset, all statistics of players for a given game
- players.csv : players details (name)
- ranking.csv : ranking of NBA given a day (split into west and east on CONFERENCE column
- teams.csv : all teams of NBA

## Analytical Insights

### Point Plot

<img width="936" alt="image" src="https://user-images.githubusercontent.com/20051049/236485733-c72bd621-8096-4831-b614-42b97728ccca.png">

This pointplot shows that the points scored and the assists accumulated do not have a significant impact on winning. There s however a direct impact on the point scored and the assists. The more assists you obtain, the higher the points.

### Scatter Plot

<img width="956" alt="image" src="https://user-images.githubusercontent.com/20051049/236485425-119db7ee-9c01-4d45-bcd0-d3b24be43ecd.png">

This scatter plot shows the lower you can keep your opponents field goal percentage and points, the greater your chances of winning. It has a moderate positive correlation.

## Best Model
### Classification Report
<img width="460" alt="image" src="https://user-images.githubusercontent.com/20051049/236493376-d457634c-31d7-4de3-a962-bca692c331be.png">

### Confusion Matrix
<img width="886" alt="image" src="https://user-images.githubusercontent.com/20051049/236492557-5065dfb0-8417-4633-9678-47423d6b7a8b.png">

The model I would use to predict the outcome of the team winning is the Tuned LR Model. It has the best overall accuracy by predicting the most correct wins and losses. The PCA models ran very quick and performed very well on the tuned KNN and the RF model, but gave lower results. Since accurately predicting the winner is the most important metric, the Tuned LR Model wins because it has a 99.7% accuracy. Out of 6,663 predictions it only got 20 of them incorrect. All of the errors were all false positives and in the sporting world I would think that thinking you are going to win is better than thinking you are going to lose because confidence is a key factor and you need every edge you can get.

I would recommend that teams focus on defense to keep their opponents overall field goal percentage and their points lower.  Teams should also focus on the total number of assists. Doing these things would have a direct impact on the home team winning. 
