# The impact of religiosity on economic development
## Overview

This project was developed as part of a group assignment for the "Global Firms and Global Markets" course. It provides a partial replication of the analysis conducted by Mara P. Squicciarini (2020) in her paper "Devotion and Development: Religiosity, Education, and Economic Progress in Nineteenth-Century France". To enhance my technical skills, I reproduced the original analysis, which was written in Stata, using Python.

The author examines historical records from 19th-century France to investigate the relationship between religion, education, and economic growth during the Second Industrial Revolution.

## Key Objectives
- **Replication**: Reproduce key empirical findings from Squicciarini (2020) to analyze the relationship between local religiosity and economic development.

- **Mechanism Analysis**: Investigate how religion influenced labor market outcomes, and consequently economic progress, by hindering the adoption of technical curricula in schools. Alternative mechanisms are tested to ensure robustness.

## Technical implementation
- **Econometrics techniques**: Application of OLS regressions, clustered standard errors and fixed-effects models using the  `statsmodels` library.
- **Data dictionaries**: Developed a function that extracts variable labels from `.dta` files and converts them into a DataFrame to facilitate variables exploration.
- **Visualization** : Reproduced line plots using `matplotlib` and `seaborn` to illustrate educational trends.

## Key Findings
- **The Schooling channel**: Regions with higher religiosity intensity experienced a slower adoption of technical curricula.
- **Workforce impact**: Religiously educated individuals were less likely to be employed in innovative, skill-intensive sectors, suggesting that educational content influenced the long-term industrialization process.
- **Robustness** : Findings remained consistent after controlling for  vaccination rates and fertility indices. This support the argument whereby education was a primary driver of economic progress.

## Project structure
- `main.ipynb` contains the Python code to complete the three tasks required by the assignment.
- `pyproject.toml`, created by `uv`, contains the packages used. 

# References 
Squicciarini, Mara P. 2020. "Devotion and Development: Religiosity, Education, and Economic Progress in Nineteenth-Century France." American Economic Review 110 (11): 3454–91. DOI: 10.1257/aer.20191054

