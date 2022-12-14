# M-Ligue Results Analysis

## Introduction

I am an active player of a sports version of the popular intellectual game What?Where?When? (WWW, Что?Где?Когда?, ЧГК).

During the pandemic, the online format of the game became more popular. One of the most attended tournaments is [M-ligue](https://chgk-world.ru/), where any team can register and participate in any game. I decided to make an analysis for our team.

## Problem statement

Our team participating in these online tournaments for almost a year. Games are being played every week. There is a result table for every game, but there is no summary table of all results, which is common practice for repeating championship-like tournaments.

But the most interesting part for me is how our team is answering questions: are we good at easy questions, do we answer the questions with the rating <10% (it means less than 10% of teams answered correctly)?

Overall, the purposes of the analysis are:

* creating summary table;
* understanding team's progress;
* comparing our team results to the performance of other teams;
* seeing the answers statistics after every game.

## Data sources

After every game, a result table is published on [M-Ligue platform](https://chgk-world.ru/). There is no correct answer data available on the internet, so I wrote down every answer during the games I took part in.

## Data cleaning

Results tables that are downloaded from the internet (and can be seen in _Example of Game_ results file) are not intended for analysis, so first I manipulated the data so I could build a dashboard based on it. The result of this transformation is in _Consolidated_ file.

We have also the _Answers_ table, which is connected with the _Consolidated_ table on Tournament and the Number of questions. Additionally, we have a _Team list_ table with the number of players on our team, who participated in games.

The process of transforming downloaded file with Results is [here (ipynb format)](https://github.com/marsel-khusnutdin/M-Ligue/blob/main/M-ligue%20results.ipynb).

## Data visualization

![Visual 1](https://user-images.githubusercontent.com/72653236/182588458-d856eb3d-73f8-47c1-ba03-e943329f5672.JPG)


![Visual 2](https://user-images.githubusercontent.com/72653236/182588471-7b600cd9-5166-48d0-a653-5b97a49df0ca.JPG)

[Interact with the dashboard on the Tableau Public here](https://public.tableau.com/app/profile/marsel.khusnutdinov7184/viz/M-LigueResults2022/DashboardMain?publish=yes)

## Conclusions

1. There is a small trend for progress in the game. But this, unfortunately, does not apply to league finals - tournaments with 48 questions (red dots and trend line). For some reason, we are playing them worse and worse. Either there is not enough stamina, or this is due to the fact that not everyone plays to the end.

    ![Visual 3](https://user-images.githubusercontent.com/72653236/182592848-0ebfcb63-6ffc-49f4-a3d1-b445fcdf0405.JPG)

2. Starting from the middle of the available observations (i.e. starting from May) we began to occasionally take highly rated questions (questions answered by <10% of the teams). May-July there were 3 such questions, before that = 0.

    ![Visual 4](https://user-images.githubusercontent.com/72653236/182593504-96ddac30-3206-4e8c-899b-3f5241aa6693.JPG)


4. We play simple tournaments better than complex ones (relative to other teams, of course). Our two most successful wagers - June 3 and July 2 - are relatively simple packages.
5. I was sure that we take catastrophically few rating questions. But it turned out that this was not the case. Teams comparable to us in terms of level take slightly less highly rated questions. But they are better with questions of medium complexity (rating = 50-60%)
6. There is a correlation between the number of players who took part in a game and the result. Most of our unsuccessful games were performed with 5 team members (red rectangle). The most successful games were performed by the number of players = 6 (green rectangle).

    ![Visual 5](https://user-images.githubusercontent.com/72653236/182594010-042d3624-663a-4ced-87a9-fb60738b9d2f.JPG)

## Recomendations

It is vital for the team to play in full team composition. Also, it makes sense to have long pieces of training to develop stamina. There are definitely several domains that can be assigned to different team members so they closed the lack of knowledge. The clear examples of such lacks are medieval history and ancient greek and biblical stories in art.
