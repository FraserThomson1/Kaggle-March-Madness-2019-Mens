# Kaggle-March-Madness-2019-Mens
a regression approach to the 2019 kaggle mens march madness competition

this repository is based on the kaggle 2019 men's march madness machine learning competition

MODELS:
my first model calculates average of advanced stats for each team for every season, and then based on which year to predict, i extract a training set using regular season winning margins as labels and differnece in season average of advanced stats for past 3 year as features.
then it is fit to a linear regression to predict the winning margins for every possible matchup of that year using the season averages for teams in that year. and the produced predicitons of the winning margins are used to create a winning probability using an optimised wieght.

a second model is based on a regression model by simply using the seed differences of the two teams in a matchup and producing a probability using another weight.

the two probabilities are then averaged to produce the final winning probabilities of the matchups.

EXPLANATION:
The advanced stats were selected according to their corrolations to how far teams advance in that year. and a model based on this model would be better at predicting upsets as it does not use seed as a feature.
Seed difference is a good feature that has a high correlation with a teams performance, hence a balanced model is attempted to be produced by combining both season average stats and seed differences.
