# Replicating "How Do Voters Respond to Information?" (Kendall et al., 2015)

## Overview

This folder has a Python-based replication of the key findings from “How Do Voters Respond to Information? Evidence from a Randomized Campaign,”. The original replication was done in Stata, but this project shows how the same econometric analysis can be done in Python.
## Objective

This project originated as an academic assignment, where the goal was to replicate the findings of a published Randomized Controlled Trial (RCT). To bridge the gap between academic research and industry standards, I took the initiative to translate the original Stata-based methodology into a Python workflow.

The primary objective of this repository is to practice technical skills. Specifically, it shows the ability to:
- **Validate Experiments**: Run ex-ante balancing tests to rigorously verify randomization protocols.
- **Implement Statistical Models**: Apply Ordinary Least Squares (OLS) and probability models, adjusting for clustered robust standard errors.
- **Communicate Results**: Generate clear regression tables using stargazer to present statistical findings effectively.
- 
## The Data

The analysis relies on two primary datasets, based on the 2011 municipal elections in Arezzo, Italy:
1. **Aggregate Data (`aggregate.dta`)**: Precinct-level data (95 observations) containing official voting outcomes, treatment assignments, and historical electoral variables.
2. **Individual Data (`individual.dta`)**: Survey-level data (1,455 observations) collecting demographics, prior beliefs, and self-reported voting declarations.

*Note: The raw `.dta` files are read directly into pandas DataFrames, extracting Stata variable labels for clear data dictionaries.*

## Technologies & Libraries Used

* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Econometric Modeling:** `statsmodels` (OLS, formulas, clustered standard errors)
* **Result Formatting:** `stargazer` (for publication-quality regression tables)
* **Environment:** Jupyter Notebook (`.ipynb`)

## Methodology & Key Steps

1. **Data Ingestion & Label Extraction:** Parsing Stata files to retain metadata and variable labels for interpretability.
2. **Randomization Validation:** Running regressions on predetermined variables (e.g., historical voting patterns, age, education) against treatment dummies to confirm the ex-ante balance of the experiment.
3. **Aggregate Treatment Effects:** Estimating the impact of different campaign messages (Valence vs. Ideology) and delivery methods (Phone vs. Mail) on voter turnout and incumbent vote share.
4. **Individual-Level Evidence:** Validating aggregate findings using individual survey data.

## Key Findings

Replicating the authors' original findings, the analysis confirms that:

* **Content Matters:** Campaign messages emphasizing the incumbent's *valence* (competence and effort) significantly increased the incumbent's vote share.
* **Medium Matters:** Phone calls were a highly effective delivery mechanism, while direct mailers had negligible or statistically insignificant effects on voting choices.
* **Ideology vs. Competence:** Ideological messages did not translate into a statistically significant advantage compared to the control group, highlighting a stronger voter responsiveness to verifiable competence.
