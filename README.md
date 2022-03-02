# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
<p align="center">
<b>Output from the linear regression</b></br>
    <img src="https://raw.githubusercontent.com/davidbaek90/MechaCar_Statistical_Analysis/main/4.PNG">
</p>

- The variables that provided a non-random amount of variance to the mpg are: 1. vehicle_length with a p-value of 2.60e-12, and 2. ground_clearance with a p-value of 5.21e-08.
- The slope of the linear model should be consiered non-zero, there are three coefficient that contribute to non-zero slope: 1. vehicle_length, 2. ground_clerance, and 3. AWD.
- Since the R-squared value is 0.7149. Which means roughly 71% of the variability of our depends variable is explained using linear model. This model would be relatively effective.

## Summary Statistics on Suspension Coils

The Suspension_Coil dataset has been processed based on all manufacturing lots and summary by individual lots.

<p align="center">
<b>total_summary</b></br>
    <img src="https://raw.githubusercontent.com/davidbaek90/MechaCar_Statistical_Analysis/main/3.PNG">
</p>

<p align="center">
<b>lot_summary</b></br>
    <img src="https://raw.githubusercontent.com/davidbaek90/MechaCar_Statistical_Analysis/main/2.PNG">
</p>

When the entire manufacturing lots is observed, the variation of PSI is 62.29, which is well within the required 100 PSI. Contrastingly, when you obseve the variation of PSi in each individual lot, there is a significant varaition in the PSI for Lot3. This would fail the 100 PSI variation criteria.

## T-Tests on Suspension Coils

<p align="center">
<b>lot_summary</b></br>
    <img src="https://raw.githubusercontent.com/davidbaek90/MechaCar_Statistical_Analysis/main/1.PNG">
</p>

- For the first test (all manufacturing lots), the sample mean is 1498.78. The sample mean is not different from the population mean. The p-value is higher than 0.05. Null hypothesis cannot be rejected.

 -For the second test (lot 1), the sample mean is 1500. The sample mean is different from the population mean. The p-value is much higher than 0.05. Null hypothesis cannot be rejected.

- For the third test (lot 2), the sample mean is 1500.2. The sample mean is different from the population mean. The p-value is much higher than 0.05. Null hypothesis cannot be rejected.

- For the forth test (lot 3), the sample mean is 1496.14. The sample mean is little less different from the population mean. The p-value is lower than 0.05. Null hypothesis can be rejected. This lot requires further evaluation or be neglected.

## Study Design: MechaCar vs Competition
In order to quantify how the MechaCar performs against the competition, we can perform additional analysis on the following metrics:
- Carbon dioxide emission rating
- Fuel economy (gas/electric/combined)
- Safety rating
- Acceleration (0-100km)
- Max. Towing Capacity Weight
- # of seats
- Truck / Boot capacity
- Weight-power output ratio

Null hypthosis is that above mentioned metrics for MechaCar prototype is simiar from the competitiors' vehicles. A alternative hypothesis that the MechaCar protype outperforms or underperforms on the metrics when compared to competitors' vehicles.

One-Way ANOVA would be the recommended test to test the hypothesis. We can compare the means of the metrics to determine whether there is a statistical evidence that the vehicle manufacturers' metrics are significantly different.

The car safety rating data is available in IIHS test database. Fuel economy of all the vehicles are available in www.fueleconomy.gov in MPG. Acceleration, maximum towing capacity, # of seats, trunc/boot capacity and weight-power ratio are availble under specification section in the manufacturers' website.
