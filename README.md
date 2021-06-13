# MechaCar Analysis

## Linear Regression to Predict MPG

After performing a (multiple linear regression)[link], we can determine that vehicle weight, spoiler angle and drivetrain (AWD) provided non-random amounts of variance to the mpg values in the dataset. The slope of the linear model is not zero, because our p-value is smaller than 0.05, therefore we can reject the null hypothesis that all these factors contribute to mpg. 

Looking at the individual p-values, vehicle length and ground clearance are significant, while vehicle weight, spoiler angel and drivetrain are not significant. Logically speaking, it makes sense that spoiler angle and drivetrain should have less of an impact on mpg, but vehicle weight typically plays a huge part in mpg, therefore the linear model is not effective at predicting mpg of MechaCar prototypes. 

## Summary Statistics on Suspension Coils

By looking at the (total summary)[link], we can see that the population variance is 62.29356 per square inch, which does not exceed 100 pounds per square inch. While the overall summary may seem like the current manufacturing standards are being met, a closer look at each (individual lot)[link] reveals a different story. Variances for Lot 1 and 2 are 0.98 and 7.47 respectively, but Lot 3 is showing variance of 170, which exceeds manufacturing standards and needs to be examined. 

## T-Tests on Suspension Coils

The first analysis conducted to find out whether the PSI for all manufacturing lots is statistically different from the population mean of 1500. Looking at the (result)[link], a p-value of 0.06 indicates that we cannot reject the null hypothesis and therefore the PSI for all manufacturing lots is not statistically different from 1500. 

The (second analysis)[link] was conducted on Lot 1 and we found a p-value of 1, which means we cannot reject the null hypothesis. The analysis for (Lot 2)[link] and (Lot 3)[link] had p-values of 0.6072 and 0.04168 respectively. Since Lot 2's p-value is greater than 0.05, we cannot reject the null hypothesis, however Lot 3's p-value is smaller than 0.05, therefore we can reject the null hypothesis and the PSI for Lot 3 is statistically different than the population mean of 1500. 


## Study Design: MechaCar vs Competition

A statistical study that can be conducted is on maintenance cost between MechaCar prototype vs. competitors. We already have data for MechaCar such as vehicle weight and length, ground clearance and drivetrain and the same data can be collected for competitors to be used in this study. The null hypothesis can be that these factors contribute to maintenance cost, the alternate hypothesis is that these factors do not contribute to maintenance cost. 

This study can be conducted using Student's T Test, similar to how we conducted the test on PSI across different manufacturing lots. We can collect data on the average annual maintenance cost for a particular type of vehicle, such as a sedan, SUV, truck etc. From there, we can conduct our study similar to the mpg study we did in this challenge except this time we will look at the mean maintenance cost. We can use subset again for each competitor and see how they compare with the mean and form our conclusion whether our factors contribute to maintenance cost. 

