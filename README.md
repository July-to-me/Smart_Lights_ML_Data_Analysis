# Smart_Lights_ML_Data_Analysis
This project is from one of my previous courses during College. It focuses on the Smart Lights Dataset from Kaggle. This was my first attempt at looking into a dataset that contains over 10,000 data points.  

## Objective

In this project, I wanted to see if one can predict a home's affluence based on its energy usage along with other variables. 
1. Getting the data via Kaggle, and loading it in Google Colab (so I can access it on multiple devices).
2. Converted the string of time in an actual time thanks to datetime. 
3. Randomly sampling data in order to conduct partial Exploratory Data Analysis.
4. I created various graphs thanks to Seaborn and Matplotlib in order to see the difference between each home's usages.
5. I then used statistical techniques such as K-Means clustering, random forest, and logistic regression to answer my questions about predicting a home's affluence.

## Dataset

I've used a dataset that I've found in Kaggle. 
More info about the dataset can be found here:
- Website: https://www.kaggle.com/datasets/jeanmidev/smart-meters-in-london


## Dataset

This dataset contains 1442772 rows and 3 columns (originally) for the variables listed below. 

Variable  |Description |
-----|-----|
LCLid| The corresponding household id |
Energy(kWh/hh)|The amount of energy used on half-hourly |
Month| The current month of the energy being used |
Day_of_month |The day of the month that the data was being recorded |
Time| The time is used in order to keep track of the energy used half-hourly
Weekday | The day of the week that the day was on 
Acorn_grouped| What type of affluent classification the household is considered
File|Which file we can find the household in
StdorToU |The tariff being applied on that household
Legendary|This is a True/False statement that says if a Pokemon is a legendary Pokemon or not. 
