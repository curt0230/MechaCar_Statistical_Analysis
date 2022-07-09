# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
A linear regression was performed on the MechaCar gas mileage data to determine the impact of fuel efficiency based on vehicle length, weight, spoiler angle, ground clearance, and drive train.  The regression test resulted in the following findings:

![summary_statistics.png](/resources/summary_statistics.png)

* Vehicle_weight, spoiler_angle and AWD appear to be non-random based on the data sample. The most random factors appear to be ground_clearence and vehicle_length
* Since p-value is less than zero (5.35e-11), the slope is lower than the level of significance.  This indicates the null hypothesis can be rejected, or that there is a statistically significant correlation between at least some values.
* The R squared value is 71.49% which implies that roughly 72% of the time the predictions will be correct using the linear model, which means that 28% of the time the prediction will be incorrect.  A more effective model could be trained.

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Overall this design specification is met based on PSI summary statistics.  
![psi_total_summary.png](/resources/psi_total_summary.png)

However, While lots 1 and 2 closely adhere to the specifications as indicated by very low variances, lot 3 exceeds tolerance and should be closely inspected and potentially rejected.
![psi_lot_summary.png](/resources/psi_lot_summary.png)


## T-Tests on Suspension Coils
briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

A cumulative t-test review of the suspension coils across all manufacturing lots indicates they are not significantly different than the population mean and thus they are within the standard based on the p-value.
![overall_t_test_results.png](/resources/overall_t_test_results.png)

A cumulative t-test review of the suspension coils manufacturing lot 1 indicates they are not significantly different than the population mean and thus they are within the standard based on the p-value.
![lot1_t_test_results.png](/resources/lot1_t_test_results.png)

A cumulative t-test review of the suspension coils manufacturing lot 2 indicates they are not significantly different than the population mean and thus they are within the standard based on the p-value.
![lot2_t_test_results.png](/resources/lot2_t_test_results.png)

A cumulative t-test review of the suspension coils manufacturing lot 3 indicates they are significantly different than the population mean and thus they exceed the standard based on the p-value.  This lot should be closely inspected and potentially rejected.
![lot3_t_test_results.png](/resources/lot3_t_test_results.png)


## Study Design: MechaCar vs Competition
Consumers consider many factors when purchasing a new vehicle.  Metrics around reliability, economy, cargo space and comfort, and speed and performance carry different weight depending on the customer and their lifestyle.  MechaCar, being an innovative take on a highly efficient multi-use vehicle, should be evaluated based on total cost of ownership.  The hypothesis is that MechaCar has a lower total cost of ownership than competitors in its class.


A two-sample t-test could be used to compare fuel efficiency and standard maintenance expenses to similar vehicles built by other manufacturers.  Data points would include:
 * Miles per gallon for both city and highway driving
 * Oil changes
 * Transmission/drive train service
 * Air filter replacements
 * Brake maintenance
 * Other standard maintenance (summarized)
 
The data points for each manufacturer including MechaCar should be summarized based on the average length of ownership, and maintenance frequency as prescribed by each manufacturer assuming average driving conditions by the consumer.  Pricing should be based on average dealership service department pricing across all manufacturers.
