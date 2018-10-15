# Football match prediction

I would like to create a neural network that would be able to predict the outcome of a football game

I use this great dataset : [https://www.kaggle.com/hugomathien/soccer/home](https://www.kaggle.com/hugomathien/soccer/home)

What I would like to see is if a team needs to play with possession or have tall players to win a game

### Data

The original sqlite database is not on the github repository, you have to download it by yourself on the kaggle website

For this project, I will use the Match table which contains a lot of informations
I'll get rid of the betting values in order to not be influenced by this
I need to get the matchs that have at least the id of the players (home_player_1, away_player_1)
The possession, shoton and all those attributes should be needed also but need to see how they are formatted
Not sure if the home and away ids are needed in order to use the team_attributes
Not sure that their positions should be useful
We don't take individuals statistics, we average players data

Final ideal data :
GoalDifference | HomePlayerHeight | HomePlayerWeight | HomePlayerOverallRating...

### Training

Multiple models can be used
It's a simple regression problem
I'll use a deep learning approcah with Keras and a simpler regression approach using scikit-learn
