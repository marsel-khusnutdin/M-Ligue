# M-Ligue Results Tournament

## Introduction

I am an active player of a sport version of the popular intellectual game What?Where?When? (WWW, Что?Где?Когда?, ЧГК).

During the pandemic online format of the game became more popular. One of the most attended tournaments is [M-ligue](https://chgk-world.ru/), where any team can register and participate in any game.

## Problem statement

Our team participating in these online tournaments for almost a year. Games are being played every week. There is a result table for every game, but there is no summary table of all results, which is common practice for repeating championship-like tournaments.

But the most interesting part for me is that how our team is answering a questions: are we good at easy questions, do we answer on the questions with the rating <10% (it means less than 10% of teams answered correctly).

Overall, the purposes of the analysis are:

* creating summary table;
* understanding team's progress;
* comparing our team results to the performance of other teams;
* seeing the answers statistics after every game.

## Data sources

After every game a result table is published on [M-Ligue platform](https://chgk-world.ru/). There is no correct answers data available on the internet, so I wrote down every answer during the games I took part in.

## Data cleaning

Results tables which are downlaoded from the internet are not intended for analysis, so first I manipulated the data so I could build dashboard based on it. We have also Answers table, which is connected with Results table on Tournament and Number of question. Additionally, we have a table with the number of players of our team, who participated in games.

## Data visualization

![Visual 1](https://user-images.githubusercontent.com/72653236/182588458-d856eb3d-73f8-47c1-ba03-e943329f5672.JPG)


![Visual 2](https://user-images.githubusercontent.com/72653236/182588471-7b600cd9-5166-48d0-a653-5b97a49df0ca.JPG)

## Conclusions

1. There is a small trend for progress in the game. But this unfortunately does not apply to league finals - tournaments with 48 questions (red dots and trend line). For some reason, we are playing them worse and worse. Either there is not enough stamina, or this is due to the fact that not everyone plays to the end.

    ![Visual 3](https://user-images.githubusercontent.com/72653236/182592848-0ebfcb63-6ffc-49f4-a3d1-b445fcdf0405.JPG)

2. Starting from the middle of the available observations (i.e. starting from May) we began to occasionally take highly rated questions (questions answered by <10% of the teams) . May-July there were 3 such questions, before that = 0.

    ![Visual 4](https://user-images.githubusercontent.com/72653236/182593504-96ddac30-3206-4e8c-899b-3f5241aa6693.JPG)


4. We play simple tournaments better than complex ones (relative to other teams, of course). Our two most successful wagers - June 3 and July2 - are relatively simple packages.
5. I was sure that we take catastrophically few rating questions. But it turned out that this was not the case. Teams comparable to us in terms of level take slightly less highly rated questions. But they are better with questions of medium complexity (rating = 50-60%)
6. There is a correlation between the number of players who took part in a game and the result. The most of our unsuccessful games were performed with 5 team members (red rectangle). The most succesful games were performed by the number of players = 6 (green rectangle).

    ![Visual 5](https://user-images.githubusercontent.com/72653236/182594010-042d3624-663a-4ced-87a9-fb60738b9d2f.JPG)

## Recomendations

It is vital for team to play in full team composition. Also it makes sense to have long trainings to develop stamina. There are definitely several domains that can be assigned to different team members so they closed the lack of knowledge. The clear examples of such lacks are medieval history and ancient greek and biblical stories in art.




