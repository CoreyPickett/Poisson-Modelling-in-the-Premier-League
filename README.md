# 🥅 Poisson Modelling in the English Premier League

A statistical modelling project investigating whether goals scored in the 2023–24 English Premier League season follow a Poisson distribution. The project applies maximum likelihood estimation, QQ‑plots, goodness‑of‑fit tests, and confidence intervals to evaluate the suitability of the Poisson model.
Completed as part of the second‑year university statistics course "Statistical Inference".

## 💻 Technologies

- R
- R markdown

## 🚀 Features

- Scrapes EPL match data using _worldfootballR_ library
- Cleans and transforms data into long format
- Maximum likelihood estiamtion of Poisson rate parameters
- QQ-Plot for visual assessment
- Kolmogorov-Smirnov and Chi-squared goodness-of-fit tests
- Likelihood-based confidence intervals using Newton-Raphson method

## 📋 The Process

The project investigates whether the number of goals scored by home and away teams in the EPL can be modelled using a Poisson distribution, as goals are independent events occurring at a constant rate.

Using the worldfootballR package, we scraped all match results from the 2023–24 EPL season and randomly sampled 50 matches for analysis. The data was reshaped into a long format to allow separate modelling of home and away goals.

We estimated the Poisson rate parameters for both home and away teams using maximum likelihood estimation, followed by assessing the model fit using:
- **QQ-Plots**
- **Kolmogorov-Smirnov Tests**
- **Chi-squared Goodness-of-fit Tests**

A 95% confidence interval was then constructed using likelihoods from the Newton-Raphson method.

## 🧠 What I learned

- Scraping and sturctuing real-world data through R packages
- Applying maximum likelihood estimation to discrete distributions
- Constructing QQ‑plots and interpreting deviations from theoretical models
- Implementing the Newton–Raphson method for confidence intervals

## 🙋‍♂️ My Contribution:
This project was compelted as a team of three, with my main contributions including:
- Writing the mathematical notation used within the report
- Deriving the maximum likelihood estimate
- Constructing the QQ-plot used in the final report

## 📊 Key Results

- Estimated Scoring rates: **Home** = 1.84, **Away** = 1.08
- QQ-Plots show strong alignment with model
- Goodness-of-fit shows no evidence of assumption violations
- 95% confidence intervals: **Home** = (1.668, 1.938), **Away** = (1.360, 1.605)
- Supports home field advantage

## 📈 Future Improvements

- Analyse full season rather than sample
- Compare Poisson with alternative models
- Extend analysis to multiple seasons, or different leagues
