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

### Bar Plot #1

<img width="855" alt="image" src="https://github.com/jaytrey777/NBA-Home-Team-Wins/assets/20051049/5b087acd-9b63-4fd9-8732-e8514371fff0">

This Barchart shows the top 10 teams with the highest scoring average at home. The Houston Rockets average the most points at home at around 140. They would be a tough opponent to face on their home court.

### Bar Plot #2

<img width="799" alt="image" src="https://github.com/jaytrey777/NBA-Home-Team-Wins/assets/20051049/0a9f0d48-4111-44c8-9fc1-eb867d3871c1">

This Barchart shows the top 10 teams with the highest scoring average away from home. The Utah Jazz average the most points on the road around 125. They would be a tough opponent to face on the road.

### Bar Plot #3

<img width="951" alt="image" src="https://github.com/jaytrey777/NBA-Home-Team-Wins/assets/20051049/67cb91fa-9819-4bc8-99a8-f3fed12ecb43">

This bar plot shows the top 10 teams that have the highest point differential scoring at home vs away. The Indiana Pacers have a scoring differential of almost 40 point at home. They are lot better at home team than they are on the road.

## Best Model
### Classification Report
<img width="471" alt="image" src="https://github.com/jaytrey777/NBA-Home-Team-Wins/assets/20051049/57e9848a-1020-4988-a8dc-aa584ad4682c">

### Confusion Matrix
<img width="853" alt="image" src="https://github.com/jaytrey777/NBA-Home-Team-Wins/assets/20051049/7b03992c-fd3e-40c5-a466-f4ea60618777">

The model I would use to predict the outcome of the team winning is the Tuned LR Model. It has the best overall accuracy by predicting the most correct wins and losses. The PCA models ran very quick and performed very well on the tuned KNN and the RF model, but gave lower results. Since accurately predicting the winner is the most important metric, the Default LR Model wins because it has a 87.1% accuracy. Out of 6,663 predictions it only got 857 of them incorrect. There were 397 false negatives and 460 false positives. All of the models gave me similar results but this one gave me the best values for false negatives.

I would recommend that teams focus on defense to keep their opponents overall field goal percentage and their points lower.  Teams should also focus on the total number of assists. Doing these things would have a direct impact on the home team winning. 
