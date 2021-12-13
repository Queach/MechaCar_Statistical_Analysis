# R Analysis

## Overview of Project
An analysis of car data on RScript

### Purpose
The purpose of this analysis is to use RScript to create a statistical analysis

## Linear Regression to Predict MPG
Vehicle weight, spoiler angle, and AWD variables provided a non-random variance to the mpg values.

The slope of the linear model is not considered to be zero, the R-squared value is 0.71 and there is a correlation between the dependant and independant variables

Because the R-squared value is 0.71 the linear model does a good job at predicting mpg of prototypes

![results](https://raw.githubusercontent.com/Queach/MechaCar_Statistical_Analysis/main/resources/6276f41f0e9d9a90c106e05d7698ea35.png "results")

## Summary Statistics on Suspension Coils

Lots 1 & 2 meet the design specifications but Lot 3 fails to meet the variance of under 100 pounds per inch.
All together they meet the specification with a variance of 62.2 but Lot 3 individually fails with a variance of 170.2

![results](https://raw.githubusercontent.com/Queach/MechaCar_Statistical_Analysis/main/resources/7a0db2f96d2f50789a5c9fcb6024a4e0.png "results")

![results](https://raw.githubusercontent.com/Queach/MechaCar_Statistical_Analysis/main/resources/3dfa589f8e20551adb47127c1922a788.png "results")

## T-Tests on Suspension Coils

When it comes to all lots together, we do not have sufficient information to reject the null hypothesis when using a normal level of importance, as the p-value is 0.06.
Lots 1 and 2 also reject the null hypothesis with p-values over 0.05.
Lot 3 cannot reject the null hypothesis with a p-value of 0.04168, therefore the variance in manufacturing fails to meet specifications.

## Study Design: MechaCar vs Competition

To determine if MechaCar performs against competition, a two-sample test should be done using MechaCars data against a competitors.
Metrics of the data set should include fuel-effciency and maintenance cost vs the price of the vehicle.

Null hypothesis: MechaCar underperforms against it's competitors and has worse fuel-effciency and maintenance cost vs overall price compared to it's competitors.

Alternate hypothesis: MechaCar outperforms against it's competitors and has better fuel-effciency and maintenance cost vs overall price compared to it's competitors.
