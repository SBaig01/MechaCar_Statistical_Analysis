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
Based on the Individual Lots data (see below), **Lot 1 and Lot 2** variance are **within the design specification** while the **Lot 3** variance is **NOT**. 

![Lot Summary](https://github.com/SBaig01/MechaCar_Statistical_Analysis/blob/d6c66cc9e314491c85ca56c80dfbb9e79a23f655/Lot%20Summary.png)
