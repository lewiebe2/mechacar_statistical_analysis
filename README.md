# MechaCar Statistical Analysis

## Linear Regression to Predict MPG

Using R and RStudio, a multiple linear regression model was created for the MechaCar MPG dataset to predict the relationship between MPG and five metrics: vehicle length, vehicle weight, spoiler angle, ground clearance, and drivetrain. 

The results are as follows:

![](resources/deliverable1_lm_output.PNG)


*1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?*

Vehicle length and ground clearance both provided non-random amounts of variance to the mpg values in the dataset.

*2. Is the slope of the linear model considered to be zero? Why or why not?*

The slope of the multiple linear regression model is not considered to be zero since the r-squared value is 0.71 and the p-value is 5.35e-11, which is much smaller than the assumed significance level of 0.05%.

*3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?*

The linear model predicts mpg of MechaCar prototypes effectively since the r-squared value is 0.71, meanihng about 71% of the variablilty of mpg is explained using this linear model, and the p-value is significant.

## Summary Statistics on Suspension Coils

*The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?*

**Total Summary**

![Total Summary](resources/deliverable2_total_summary.PNG)

The current total manufacturing data meets the design specifications with a variance of 62.29.

**Lot Summary**

![Total Summary](resources/deliverable2_lot_summary.PNG)

However, the current lot manufacturing data shows that Manufactoring Lot 3 does not meet the design specifications with a variance of 170.23. Manufacturing Lots 1 and 2 meet the design design specifications, so corrective action is only needed at Manufactoring Lot 3.

## T-Tests on Suspension Coils

![](resources/deliverable3_all_lots_ttest.PNG)

The t-test comparing the mean PSI across all manufacturing lots to the population mean of 1,500 pounds per square inch shows that the sample mean (1498.78) is statistically different.

![](resources/deliverable3_Lot1_ttest.PNG)

The t-test comparing the mean PSI for Lot 1 to the population mean of 1,500 pounds per square inch shows that the sample mean (1500) is statistically equivalent to the population mean.

![](resources/deliverable3_Lot2_ttest.PNG)

The t-test comparing the mean PSI for Lot 2 to the population mean of 1,500 pounds per square inch shows that the sample mean (1500.2) is statistically different.

![](resources/deliverable3_Lot3_ttest.PNG)

The t-test comparing the mean PSI for Lot 3 to the population mean of 1,500 pounds per square inch shows that the sample mean (1496.14) is statistically different.

## Study Design: MechaCar vs Competition

*What metric or metrics are you going to test?*

My statistical study will test the United States cost of the MechaCar against the competition vehicles in the same size class and model year, since cost is typically the highest interest to a consumer.

*What is the null hypothesis or alternative hypothesis?*

**Null hypothesis:** There is no statistical difference between the observed United States MechaCar sample mean and its presumed vehicle size class population mean cost in the same model year.

**Alternative hypothesis:** There is a statistical difference between the observed United States MechaCar sample mean and its presumed vehicle class population mean cost in the same model year.

*What statistical test would you use to test the hypothesis? And why?*

My statistical study will use the one-sided t-test to compare the United States MechaCar mean cost (sample) to the United States mean cost for all vehicles in the size class (population) in the same model year. The one-sided t-test is used to help consumers evaluate the cost of the MechaCar versus competitors’ cars in the same vehicle size class and model year. 

*What data is needed to run the statistical test?*

The data needed to run the statistical test is the cost of the MechaCar across the United States and the cost of competitors cars in the same vehicle size class and model year across the United States.


