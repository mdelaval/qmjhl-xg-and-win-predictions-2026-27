# qmjhl-xg-and-win-predictions-2026-27

*This repository is part of my capstone course assignment in Toronto Metropolitan University's Big Data certificate, completed in the Fall 2026 semester.*

This project is creating an “expected goals” model using the QMJHL’s public API data. Expected goals (xG) models are a very common analytics metric in hockey, most prominently in the National Hockey League (NHL). It uses historical data to predict the probability of a shot becoming a goal, from 0% to 100%, using variables such as shot location and time between shots. Such public research into xG at the QMJHL level does not yet exist. This model will be used to evaluate player values, as well as predict results of future games.

The data comes from the QMJHL API, which is powered by HockeyTech. This data is what powers the “game centres” on the QMJHL’s league website, which provides live updates during games and archives previous games. The data displayed on each game centre page is publicly accessible in JSON format through browser inspection tools. For brevity and relevance to the project, the .csv data provided in this repository includes only shots, goals, penalties, penalty shots, and goalie changes. There are about 90 of those events per game, multiplied by 580 games in the 2026-27 regular season.

Based on previous xG work in the NHL, I will explore models such as original least squares regression, ridge regression, and extreme gradient boosting to see which method best fits the QMJHL. The xG model will power Monte Carlo simulations to simulate the remaining schedule and produce end-of-season standings and expected playoff brackets.
