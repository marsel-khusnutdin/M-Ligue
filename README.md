# M-Ligue Results Analysis

## Introduction

I actively participate in a sports version of the popular intellectual game What? Where? When?

During the pandemic, the online format of the game gained popularity. One of the most attended online tournaments is the [M-ligue](https://chgk-world.ru/), and I decided to analyze our team’s performance in this tournament.

## Problem statement

Our team has been participating in these online tournaments for almost a year, with games taking place weekly. While each game has its own result table, there is no summary table aggregating results across games—something commonly found in recurring, championship-style competitions.

What interests me most is understanding how our team performs in terms of question difficulty:

- Are we consistently good at answering easier questions?
- How do we perform on questions with a rating below 10% (i.e., questions answered correctly by fewer than 10% of teams)?

## Objectives of the Analysis

- Create a summary table of game results
- Track the team’s progress over time
- Compare our performance to that of other teams
- Review statistics for each game, especially regarding question difficulty

## Data sources

After each game, a results table is published on the [M-Ligue platform](https://chgk-world.ru/).

## Data cleaning

The results tables downloaded from the internet (see “Example of Game Results” file) are not structured for analysis. Therefore, I first transformed the data to build a usable dashboard. The cleaned and structured data is available in the “Consolidated” file.

Additionally, we have:

- An Answers table, linked to the Consolidated table by tournament and question number
- A Team List table that records how many team members participated in each game

The full data transformation process is documented in a [Jupyter notebook (.ipynb format)](https://github.com/marsel-khusnutdin/M-Ligue/blob/main/M-ligue%20results.ipynb).



## Data visualization

![Visual 1](https://user-images.githubusercontent.com/72653236/182588458-d856eb3d-73f8-47c1-ba03-e943329f5672.JPG)


![Visual 2](https://user-images.githubusercontent.com/72653236/182588471-7b600cd9-5166-48d0-a653-5b97a49df0ca.JPG)

[Interact with the dashboard on the Tableau Public here](https://public.tableau.com/app/profile/marsel.khusnutdinov7184/viz/M-LigueResults2022/DashboardMain?publish=yes)

## Key Findings

- **Team Progress:** There is a slight upward trend in our performance. However, this does not apply to league finals (tournaments with 48 questions). In fact, our performance in these has declined over time (see red dots and trend line). This might be due to fatigue or incomplete team participation.

    ![Visual 3](https://user-images.githubusercontent.com/72653236/182592848-0ebfcb63-6ffc-49f4-a3d1-b445fcdf0405.JPG)

- **Challenging Questions:** Starting in May, we began to occasionally answer highly difficult questions (answered correctly by <10% of teams). From May to July, we correctly answered 3 such questions, compared to 0 before that.

    ![Visual 4](https://user-images.githubusercontent.com/72653236/182593504-96ddac30-3206-4e8c-899b-3f5241aa6693.JPG)


- **Performance by Tournament Complexity:** We perform better in simpler tournaments, relative to other teams. Our most successful games—on June 3 and July 2—were from relatively easy question sets.
- **Question Rating Insights:** Contrary to my initial assumption, we don’t perform catastrophically on high-difficulty questions. Comparable teams actually answer fewer of those correctly. However, they tend to outperform us on medium-difficulty questions (50–60% correctness rate).
- **Team Composition:** There is a clear correlation between the number of players and our performance. Most of our weaker games were played with only 5 members (see red rectangle), while our strongest results came with 6 players (green rectangle).

    ![Visual 5](https://user-images.githubusercontent.com/72653236/182594010-042d3624-663a-4ced-87a9-fb60738b9d2f.JPG)

## Recomendations

- **Full Team Participation:** It’s critical to ensure all team members are present for each game.
- **Stamina Building:** Longer practice sessions may help improve performance in lengthy tournaments (like the finals).
- **Domain Expertise:** Team members should specialize in specific knowledge areas to cover existing gaps. Notable weaknesses include medieval history, ancient Greek culture, and biblical references in art.
