
# Linear Regression and Data Visualization with Seaborn

This project investigates whether higher film budgets lead to more box office revenue. The analysis uses movie budget and financial performance data scraped from [the-numbers.com](https://www.the-numbers.com/movie/budgets) on **May 1st, 2018**.

![Movies Data Visualization](https://i.imgur.com/kq7hrEh.png)

## Table of Contents

- [Introduction](#introduction)
- [Import Statements](#import-statements)
- [Data Exploration and Cleaning](#data-exploration-and-cleaning)
- [Data Type Conversions](#data-type-conversions)
- [Descriptive Statistics](#descriptive-statistics)
- [Zero Revenue Films](#zero-revenue-films)
- [Filtering on Multiple Conditions](#filtering-on-multiple-conditions)
- [Unreleased Films](#unreleased-films)
- [Films that Lost Money](#films-that-lost-money)
- [Data Visualization](#data-visualization)
  - [Bubble Charts](#bubble-charts)
  - [Movie Releases Over Time](#movie-releases-over-time)
  - [Seaborn Regression Plots](#seaborn-regression-plots)
- [Linear Regression with Scikit-Learn](#linear-regression-with-scikit-learn)
- [Model Predictions](#model-predictions)
- [Conclusion](#conclusion)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Introduction

In this project, we explore the relationship between film budgets and box office revenue using data from movies released over several decades. We'll clean the data, perform exploratory data analysis, and visualize the results using Seaborn. Finally, we'll apply linear regression to estimate the revenue potential of films based on their production budgets.

## Import Statements

The following libraries are used:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.linear_model import LinearRegression
```

## Data Exploration and Cleaning

We start by loading the data, checking for missing values, duplicates, and understanding the structure of the dataset.

## Data Type Conversions

We clean the monetary columns by removing `$` and `,`, then convert them to numeric types. We also convert the `Release_Date` column to a Pandas Datetime format.

## Descriptive Statistics

We calculate key statistics, such as average production budgets, average worldwide gross, and identify films that lost money.

## Zero Revenue Films

Here, we analyze films that grossed $0 domestically or worldwide, and investigate the highest budget films that failed to generate revenue.

## Filtering on Multiple Conditions

We filter the dataset to identify international releases and unreleased films as of May 1st, 2018.

## Unreleased Films

We remove films that hadn't been released as of the scrape date from our analysis.

## Films that Lost Money

We calculate the percentage of films where production costs exceeded worldwide gross revenue.

## Data Visualization

### Bubble Charts

We create bubble charts to visualize the relationship between production budgets and worldwide gross revenue.

### Movie Releases Over Time

We plot movie releases over time to observe trends in budget and revenue.

### Seaborn Regression Plots

Using Seaborn, we plot linear regression lines to explore the correlation between film budgets and revenue for both old and new films.

## Linear Regression with Scikit-Learn

We perform linear regression analysis using Scikit-Learn to quantify the relationship between production budget and revenue. We calculate the intercept, slope, and R-squared values for both old and new films.

## Model Predictions

We use the linear model to predict the revenue of a hypothetical film with a $350 million budget.

## Conclusion

Our analysis reveals a positive correlation between film budgets and box office revenue. However, the strength of this relationship varies between older and newer films. The linear regression model provides a tool to estimate potential revenue based on budget, though the accuracy is limited by the inherent variability in the data.

## Installation

To run this project locally, clone the repository and install the required packages:

```bash
git clone git@github.com:Prathamesh326/Linear-Regression-and-Data-Visualization-Seaborn.git
cd Linear-Regression-and-Data-Visualization-Seaborn
pip install -r requirements.txt
```

## Usage

Run the Jupyter notebook or Python script to execute the analysis. The visualizations and regression models will help you explore the relationship between movie budgets and revenue.

## License

This project is licensed under the MIT License.
