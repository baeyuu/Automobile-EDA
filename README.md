# Automobile-EDA
An Exploratory Data Analysis of an Automobile dataset

### Project Overview

This project aims to perform comprehensive data analysis on automobile data to gain insights and understand the relationships between various features and automobile prices.

### Data Source
Automobile_data: The Primary dataset used for this analysis is the "Automobile_data.csv, " which was obtained from kaggle.

### Data Columns:

- symboling: Categorical - Relative cost/prestige of the car.
- normalized-losses: Numeric - Insurance risk rating.
- make: Categorical - Car manufacturer.
- fuel-type: Categorical - Type of fuel used (gas, diesel, etc.).
- aspiration: Categorical - Engine aspiration (standard, turbo, etc.).
- num-of-doors: Categorical - Number of doors.
- body-style: Categorical - Car's body style (sedan, hatchback, etc.).
- drive-wheels: Categorical - Drivetrain (front-wheel drive, rear-wheel drive, etc.).
- engine-location: Categorical - Location of the engine (front, rear).
- wheel-base: Numeric - Distance between the front and rear axles.
- engine-size: Numeric - Engine displacement in cubic centimetres.
- fuel-system: Categorical - Fuel delivery system (multi-point injection, carburettor, etc.).
- borestroke: Categorical - Engine bore and stroke measurements.
- compression-ratio: Numeric - Engine's compression ratio.
- horsepower: Numeric - Maximum engine horsepower.
- peak-rpm: Numeric - Engine's revolutions per minute at peak horsepower.
- city-mpg: Numeric - Car's fuel efficiency in miles per gallon (city driving).
- highway-mpg: Numeric - Car's fuel efficiency in miles per gallon (highway driving).
- price: Numeric - Car's price in US dollars.

### Tools
- Python 3.x
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Numpy

### Data Cleaning
- Identified and handled missing values in the dataset by replacing numerical values with mean and categorical values with mode.
- Checked for outliers that could skew the analysis.
- Standardize and clean data formats to ensure consistency across all columns.

### Exploratory Data Analysis

The EDA involved exploring the dataset to carry out the following activities such as:
- Performed univariate analysis to understand the distribution of individual variables.
- Conducted bivariate analysis to identify relationships between pairs of variables.
- Analyzing correlations between numerical variables using correlation matrices

### Data Visualization

This was done to visually represent the data using graphs and charts to facilitate a better understanding of the patterns and trends by doing the following.

- Created histograms, bar charts, and pie charts to visualize the distributions and proportions of categorical variables.
- Generated scatter plots and line graphs to visualize relationships between numerical variables.
- Designed heatmaps and correlation matrices to visualize correlations between variables.

Includes some interesting code features

``` Python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

plt.rcParams['figure.figsize']=(23,10)
ax = sns.boxplot(x="make", y="price", data=df_automobile)

sns.catplot(data=df_automobile, y="normalized-losses", x="symboling" , hue="body-style" ,kind="point")
```
### Result and Findings

The Analysis results are summarized thus:
- Most of the cars company produces cars in the range below 25000
- Curb-size, engine size, and horsepower are positively correlated while city-mpg, highway-mpg are negatively correlated also city-mpg is negatively correlated with price as increased horsepower reduces the mileage
- More than 70 % of the vehicles have Ohc type of Engine, 57% of the cars have 4 doors, Gas is preferred by 85 % of the vehicles, Most produced vehicles are of body style sedans around 48% followed by hatchbacks 32%
- Most of the car has a Curb Weight is in range 1900 to 3100 

### Recommendation
Based on the analysis the following recommendations should be considered by the company
Vehicles within a price range lesser than 2500, OHC type engines, and gas-powered engine to maximize profits


### Refrences

1. [Kaggle](https://www.kaggle.com/datasets/kunalgupta2616/hackerearth-customer-segmentation-hackathon)
2. [Chatgpt](https://chat.openai.com/)
