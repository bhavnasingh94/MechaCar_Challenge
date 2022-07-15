# MechaCar_Challenge

# Overview
The purpose of this project is to help Jeremy by performing statistical analysis on data related to the production of MechaCar prototypes in order to provide insights to the manufacturing team.

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 

## Linear Regression to Predict MPG

The multiple linear regression analysis was performed to identify which variables in the MPG dataset predict the MPG of the MechaCar prototypes. The independent variables included in the analysis were vehicle length, spoiler angle, vehicle weight, ground clearance, & all-wheel drive. 
Due to statistical significance level of 0.05, vehicle length and ground clearance provide a non-random amount of variance to the MPG values in the dataset as shown below. Meanwhile, spoiler angle, vehicle weight, and AWD don't. The p-value for the model is much smaller than our statistical significance level of 0.05, which allows us to reject the null hypothesis that the slope of our model is zero. Even though the r-squared value of the linear regression shows that it performs well, it does not necessarily mean that the linear model predict mpg of MechaCar prototypes effectively solely because 3/5 of the independent variables in the database is not statistically significant. Further tests and data will be warranted to determine the effectiveness of prediction of the mpg.

![MechaCar_LR_Results](https://user-images.githubusercontent.com/98790082/179142725-61f02dc0-8ebd-446e-8507-a225c8afdb60.png)

## T-Tests on Suspension Coils

![ttest](https://user-images.githubusercontent.com/98790082/179144806-f12eb5a5-c93a-47f7-b2ae-4c229b10d6a4.png)

![ttest2](https://user-images.githubusercontent.com/98790082/179144807-8a7b55ec-2b00-4ed6-b392-b74d32edd2d7.png)

Lot 1 shows is highly reliable statistical match to the presumed mean PSI values across the dataset. The t-test value of 0 suggests that there is no statistically significant difference between the mean PSI of the sample and population distribution. In Lot 2, The t-test value of 0.51 suggests that there is little statistical difference between the mean PSI of the sample & population distribution. A p-value of 0.607 indicated that the null hypothesis should be accepted (Because 06.2072 > 0.5). In Lot 3 with the p-value of 0.04168 shows that the values is very less reliable and the null hypothesis should not rejected (Because 0.4 < 0.5)

## Study Design: MechaCar vs Competition

A metric to be tested? 
- Manufacture, engine/transmission, annual repair/maintenance, market/retail price, and mileage at the end-of-life of the vehile

Null hypothesis: MechaCar is worth buying as it will save consumers more money in the long-run over the car's life compared to other vehicles in the market.

Which test would you use to test the hypothesis? Multiple linear regression across these variable to find correlation and differentiate variable that are contributing to the performance outcomes as well as t-test of each variables across the manufacturer groups

Which data would you use? We need a large database on many manufacturers and consumner data information.

Link to R-Public: https://rpubs.com/bhavnasingh94/924144
