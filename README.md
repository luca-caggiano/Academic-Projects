# Quantifying the impact of religiosity on economic development
## Overview

This project was developed as part of a group assignment for the "Global Firms and Global Markets" course. It represents a replication of some analyses conduced by Mara P. Squicciarini (2020) in her paper "Devotion and Development: Religiosity, Education, and Economic Progress in Nineteenth-Century France". To enhance my coding skills, I decided to rerun the analyses, originally written in Stata, using Python.

The author employed historical records from 19th century France to examine the relationship among religion, education, and economic growth during the Second Industrial Revolution. 

## Key Objectives
- **Replication**: Reproduce key empirical findings from Squicciarini (2020) to analyze the relationship between local religiosity and economic development.
- **Analyze mechanisms**: Investigate the how religion influenced labor market outcomes, and therefore the economic progress, by hindering the adoption of technical curricula in schools. Alternative mechanisms will be tested as well.

## Technical implementation
- **Econometrics techniques**: Application of OLS regressions, clustered standard errors and fixed-effects models through `statsmodels`.
- **Data dictionary**: Developed a function that extracts variable labels from `.dta` files and convert a DataFrame to enhance variables navigation.
- **Visualization** : Reproduced line plots using matplotlib 