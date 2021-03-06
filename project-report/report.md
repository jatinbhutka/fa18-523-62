# Predict EPL results using Tweets :hand: fa18-523-62

| Manek Bahl, Sohan Udupi Rai
| mbahl@iu.edu, surai@iu.edu
| Indiana University
| hid: fa18-523-62, fa18-523-69
| github: [:cloud:](https://github.com/cloudmesh-community/fa18-523-62/blob/master/project-report/report.md)
| code: [:cloud:](https://github.com/cloudmesh-community/fa18-523-62/blob/master/project-code/code)

---

**:mortar_board: Learning Objectives**

* Learn about extracting Tweets and storing them on MongoDB
* Run Machine Learning and NLP algorithms on the data to predict soccer results

---

Keywords: Twitter API, MongoDB, Machine Learning, NLP

## Abstract

There are a lot of factors that influence the outcome of a football game. Team
statistics such as recent form, win-loss ratio, goals scored, goals conceded etc
have been proven to be useful in dictating the results of a game. These
statistics can be directly obtained from the Official EPL website, however,
there are certain other factors such as injuries, general mood of the fanbase
and sentiment of the fanbase, preparation by the team etc. which aren’t
documented in the official website. Analysis of Twitter data could prove useful
in extracting these undocumented features, using NLP models. In this paper, we
analyze the usefulness of Tweets in predicting the outcomes of games in the
English Premier League. We create three different models to predict the
outcomes, the first using the statistics available from the EPL website, the
second using only the twitter data and the third with combination of both. If
the model improves with the addition of features obtained from the twitter data,
we would be able to prove that Twitter data does increase the predictive power
of the model.

## Introduction

The English Premier League is one of the most famous and competitive football
leagues in the world. The season begins in August and ends in May in which 20
teams compete for the championship. Each team plays each of the other teams
exactly twice, Home and Away, over the course of the season. A win awards the
team with 3 points while a draw earns 1 point and a loss gives 0 points. At the
end of the season, the team with the maximum points is crowned as the champion.

Twitter is a social media website where people express their opinions about a
wide range of topics such as Politics, Sports, Religion, Entertainment etc. It
was launched in 2006 and currently has 335 Million users worldwide. Due to the
large number of users, Twitter has proven to be a reliable source of the general
opinion of the public regarding any matter. When it comes to tweets regarding
the Premier League, Twitter is being used not only by the public, but also by
the players and the club officials. Therefore, we think that tweets could
contain valuable information which could be used to improve the prediction
models.

We are choosing the English Premier League due to its globally widespread
fanbase which is active on Twitter. This provides us with a rich corpus of data
regarding the team which could be used to analyze and interpret the overall fan
sentiment for a team and other factors such as player unavailability, current
coaching style etc. which are subjective and hence not obtainable from any other
statistical sources.

For each team playing in the upcoming weekend fixtures, we are using Twitter
streaming API in Python, to monitor and extract all tweets over the course of
the entire week. This is repeated for 4-6 weeks in succession, to build the
corpus of tweets. These tweets are fed to Natural Language Processing models to
create features which serve as the predictors in the dataset. The corresponding
results of the matches will serve as the class labels. The results are only
needed for the first 4 weeks which serve as the training dataset. Supervised
Machine Learning algorithms are then trained on the training dataset. The
trained algorithms are then used to predict the unseen results of the last week
of the dataset which serves as the test data.


## Requirements

## Design 

## Architecture

## Dataset

## Implementation

## Benchmark

## Conclusion

## Acknowledgement
