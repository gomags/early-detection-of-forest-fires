# early-detection-of-forest-fires

Folder Structure:
- Algerian_Forest_Fire.ipynb: contains code for data processing and model building and results
- algerian_fires_test.csv: test set
- algerian_fires_train.csv: train set

## Problem Statement

The forest fire dataset from UCI machine learning repository contains area of forest fire and used
to predict the same. This dataset is further modified by adding a forest fire indicator variable along
with the weather data. Most of the fire management agencies use six components that account
for the effects of fuel moisture and weather conditions on fire behaviour. These codes represent
numeric ratings of moisture content of forest and floor, spread of fire, combustibility of fuels available
in forest. All of these codes are derived from meteorological readings namely temperature, relative
humidity(RH), wind speed and precipitation.

The main objective being building a system to predict the forest fire incidents in advance using
the past data, multiple analysis have to be carried out to understand data, select important features,
create new features if necessary to capture past effects. Main challenge in this task is dealing the
limited data and performing feature engineering while keeping in mind the ultimate step to output
a generalized model.

## Dataset

The dataset contains weather data from two regions in Algeria over a period of 3 months during
summer from June 1, 2012 to Sept 30, 2012. A total of 184 records from June to August in
training set and 60 records in test data of September month. The histogram on dataset says
that Temperature, RH, Ws, FFMC are normally distributed, while Rain, DMC, DC, ISI, BUI are
right skewed. The class variable is nearly balanced with 45 percent records indication no fire and
55 percent indicating fire. The BUI variable is strongly correlated with the DC and DMC from correlation 
matrix, which can be eliminated as the same information is spread betweenthe DC and DMC features.
