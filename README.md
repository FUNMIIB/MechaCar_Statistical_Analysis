# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![Linear Regression to Predict MPG](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/Linear%20Regression%20to%20Predict%20MPG.png)

**Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

The most significant variables that provided a non-random amount of variance to the mpg values in the dataset of the MechaCar are the Vehicle Length and the Ground Clearance. In the image shown above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.

**Is the slope of the linear model considered to be zero? Why or why not?**

The slope of the linear model can not be considered to be zero, because the p-value of 5.35x10-11, is lower than even an extreme level of significance, and thus the null hypothesis must be rejected meaning that the relationship between the variables and the miles per gallon is subject to more than random chance.

**Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

The prediction by this model the mpg of the MechaCar prototype is relatively effective. The r-squared value of 0.7149 indicates that the model is 71% accurate.

## Summary Statistics on Suspension Coils
![Total_summary](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/Total_summary.png)

![Lot_summary](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/Lot_summary.png)

**The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

The overall variance, as shown in the Total Summary image above, is under 100 psi and meets specifications, but one of the individual lots there has a problem. As shown in the Lot Summary stats, the variance for Lot 3 is over the acceptable threshold, at 170.28.

## T-Tests on Suspension Coils

Suspension Coils Cumulative T-test

![Suspension coils cummulative T_test1](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/Suspension%20coils%20cummulative%20T_test1.png)

Results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is high (0.0603) so we cannot reject the null hypothesis.

![Suspension coils cummulative T_test2](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/Suspension%20coils%20cummulative%20T_test2.png)

The results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is high (1) so we cannot reject the null hypothesis.

![T_test lot2](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/T_test%20lot%202.png)

The results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is high (0.6072) so we cannot reject the null hypothesis.

![T_test lot 3](https://github.com/FUNMIIB/MechaCar_Statistical_Analysis/blob/main/T_test%20lot%203.png)

The results of the T-test for the suspension coils for Lot 3 shows that they are statistically different from the population mean, and the p-value (0.0417) allows us to reject the null hypothesis. 

## Study Design: MechaCar vs Competition

**Metric to test**
Evaluate the carrying capacity of MechaCar's in cubic inches, and compare it to several competitors' vehicles.

**Null and Alternate Hypothesis**
H0: MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class 

Ha: MechaCar prototypes' average carrying capacity is statistically different than that of competitor vehicles.

**Statistical Test Used**
Two-sample t-tests.

**What data is needed**
Cubic space data from the carrying compartments of all MechaCar prototypes, and from all biggest competitor vehicles.






