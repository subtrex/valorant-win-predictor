# Valorant Win Prediction using Machine Learning

The project aims to predict the winner of a valorant match based on 2 sets of data:-

1. Player Ratings: Valorant player ratings are calculated by taking into account a variety of in-game factors like kills, deaths, assists, first bloods, multikills, clutches, spike plants/defuses, and economic situations, with a complex algorithm weighing each action to produce a single rating that represents a player's overall performance in a match; essentially, the higher the rating, the more impactful a player was considered to be. 

2. Match Statistics Data: These include the number of kills, deaths, assists, K/D ratio, average damage per round, headshot percentage, first bloods, first deaths, and average combat score.

## Tech

Python | pandas | scikit-learn | Selenium | BeautifulSoup

## Data

We have scraped data from a valorant statistics website named "The Spike" (https://www.thespike.gg/). 

For our project, we have considered matches from VCT 2021 - Stage 3 - North America - Challengers 1 - Open Qualifier (https://www.thespike.gg/events/results/vct-2021-stage-3-north-america-challengers-1-open-qualifier/839).

We scraped the data for 160 matches, with stacking the data in the following order to create the feature dataframe.

[Team_0 (the team who started in the Defender half)] [Team_1 (the team who started in the Attacker half)]
 
[Team_0 feature values] [Team_1 feature values] [Result (0 if Team_0 wins, 1 is Team_1 wins)] 
