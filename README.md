# MechaCar_Statistical_Analysis
Module 15 Challenge

## Linear Regression to Predict MPG
- **Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?** Vehicle length (value = 0.0000105 or 2.60e-12) and ground clearance (value = 0.00000184 or 5.21e-08) provide non-random amounts of variance to the mpg values. This is because they show having a significant impact on the mpg with their significance almost equal to zero.
![NonRandom_variance.png](Images/NonRandom_variance.png)
- **Is the slope of the linear model considered to be zero? Why or why not?** The slope of this linear model is not considered zero. If we look at our p-value, which is 5.35e-11, it is much smaller than the assumed significance level of 0.05% and disproves the null hypothesis.
- **Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?** When looking at the multiple R-squared value of 0.7149, we can see that this value falls between the ideal range for r-sqaured values of 0 and 1. This means that approximately 71% of the variability of our dependent variable can be explained using this multiple linear regression model.

## Summary Statistics on Suspension Coils
- **The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?** 

![total_summary.png](Images/total_summary.png)

As pictured above, we can see that the variance is 62.29356, which falls within the design specifications of not exceeding 100 pounds per square inch. Therefore, when viewing the total summary, the manufacturing data meets this design specification. While looking at the lot summaries, pcitured below, lots 1 (var=0.97959) and 2 (var=7.46939) fall within the specifications, while lot 3 exceeds those specifications. Therefore, only 2 out of the three lots meet these specifications.

![lot_summary.png](Images/lot_summary.png)

## T-Tests on Suspension Coils
![first_ttest.png](Images/first_ttest.png)

In the first t-test, we needed to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1500 pounds per square inch. As we can see the p-value is equal to 0.06028. Assuming a significance level of 0.05, we can determine that there is not sufficient evidence or it is not statistically different. Therefore, we fail to reject the null hypothesis.

In the other t-tests, we needed to determmine if the PSI for each manufacturing lot is statistically different from the population mean of 1500 pounds per square inch. Across the board, with all three individual lots, the p-value is less than 2.2e-16, which we can conclude is statistically significant. It falls within the range of being highly statistically significant, less than 0.01. With full confidence, we can reject the null hypothesis.

![lot1_ttest.png](Images/lot1_ttest.png)
![lot2_ttest.png](Images/lot2_ttest.png)
![lot3_ttest.png](Images/lot3_ttest.png)
