# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The following 2 variables provided a non-random amount of variance to the mpg values (see details below)
1) **vehicle_length**: p-value = **2.60e-12** (see below)
2) **ground_clearance**: p-value = **5.21e-08** (see below)


### Is the slope of the linear model considered to be zero? Why or why not?
The slope is **NOT** considered to be zero as the p-value is significant i.e. <0.05. This is grounds for rejecting the null-hypothesis indicating that the slope is not zero.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The multiple r-squared value is 0.7149 (see details below). This indicates that the 2 variables identified above account for almost 71% of the variance observed through this model.

  ![Stats Summary](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/1cb0e521b67fe303df807d727a3768cfee50e2f3/mecha_mpg%20Summarylm.png)

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

### Lots in Total - Does the current manufacturing data meet this design specification?
Based on the Total Summary (see below), when all lots data is combined, the variance is **62.3** which is **WITHIN** the design specification overall.

  ![Total Summary](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/d6c66cc9e314491c85ca56c80dfbb9e79a23f655/Total%20Summary.png)

### Lots Individually - Does the current manufacturing data meet this design specification?
Based on the Individual Lots data (see below), **Lot1 and Lot2** variance are **within the design specification** while the **Lot3** variance is **NOT**. 

  ![Lot Summary](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/d6c66cc9e314491c85ca56c80dfbb9e79a23f655/Lot%20Summary.png)

## T-Tests on Suspension Coils

### Lots in Total
The total mean of the sample dataset is **1498.78** and the p-value for the statistical significance testing is **0.06**. Since the p-value is not less than 0.05, we cannot reject the null hypothesis and assume that there is **no statistical difference** between the sample mean and the population mean.

  ![Total t-test](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/59ed18c7b609d0dd1026d4478300ae0fdaf689ee/One%20Sample%20t-test.png)

### Lots Individually
1) Lot1:The total mean of Lot1 is **1499.8** and the p-value for the statistical significance testing is **1**. Since the p-value is not less than 0.05, we cannot reject the null hypothesis and assume that there is **no statistical difference** between the sample mean and the population mean.
2) Lot2:The total mean of Lot2 is **1499.4** and the p-value for the statistical significance testing is **0.60**. Since the p-value is not less than 0.05, we cannot reject the null hypothesis and assume that there is **no statistical difference** between the sample mean and the population mean.
3) Lot3:The total mean of Lot3 is **1492.4** and the p-value for the statistical significance testing is **0.04**. Since the p-value is not less than 0.05, we cannot reject the null hypothesis and assume that there is **no statistical difference** between the sample mean and the population mean.

   ![Lots t-test](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/59ed18c7b609d0dd1026d4478300ae0fdaf689ee/Lot%20t-test.png)

## Study Design: MechaCar vs Competition
Consumer are interested in purchasing reliable cars that not only cost less on maintenance but have less trips to the mechanic each year. The proposed study compares the average number of trips to the mechanic between MechaCar and Competition. 

### What metric or metrics are you going to test?
The mean number of trips to the mechanic each year.

### What is the null hypothesis or alternative hypothesis?
The null hypothesis is that there is no difference in the number of trips each year between MechaCar and Competition.

### What statistical test would you use to test the hypothesis? And why?
We would use a **Two-Sample t-Test** to perform this analysis as the metric being collected is **Numerical** in nature. Since the trips would be either 1, 2, 3, etc... Also, since the trips are spaced out evenly on a scale, we could consider the data to be **Interval**.

### What data is needed to run the statistical test?
We would need to randomly select a sufficient sample of data. Once sampled, we will need the **Number of Trips to the Mechanic** as well as the year the trip was undertaken to group (or stratisfy) the results data across different model years.
