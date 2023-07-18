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

## Discovery

Here is a small conclusion that I've found based on my findings:
- Pokemon with one type from generation 5-7 has experienced a big nose dive in representation. We can also see Pokemon with two types did also suffer from not having a lot of representation as well.
- Overall, the population between one-type and two-type Pokemon does seem similar until the mentioned nose dive from generation 5-6, where two-type Pokemon have more representation in Pokemon games.
- When conducting a T-test, I found that Pokemon with two-type and one-type are statistically significant from one another. This means that Pokemon with two types, on average, had usually higher stats than pokemon with one type.
- Water types have a big representation at a whopping 10.63%, followed by Normal-types 9.40%. But when it comes to legendary Pokemon, Psychic, and Dragon-types become the most potent (16.84% and 11.05% respectively).
- Shockingly Fire types are not even the top 5 most frequent types despite being the main 3 types to be selected at the beginning of the game as a starter Pokemon. As well as not being a potent type when it comes to legendary Pokemon.
- Every 'Total' stat, on average (per generation/region), for non-legendary-pokemon has been very consistent.
- Same goes for legendary but generation 7th (Alola) has experienced an average total stat of 561 (a huge 10% decrease of the total average of all legendaries)
- Thanks to ANOVA, we now know that a lot of types do contain stats that are statistically significant from one another.
- The Attack stat/attribute for all Pokemon was statistically significant, based on regions/generations. (I assume it is because of the outliers of the different regions/generations)
- We can also see that HP and Defense were the ones that were most statistically significant across different regions(based individually per type).
- Ghost-types have a random distribution of stats than other typings. This means that there may be no way of predicting where what stat/attribute will be more prominent in the next set of generations.


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
