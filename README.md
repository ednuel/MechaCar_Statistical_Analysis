# MechaCar_Statistical_Analysis
Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
# Overall preview of the project
## Deliverable 1: Linear Regression to Predict MPG
## Deliverable 2: Create Visualizations for the Trip Analysis
## Deliverable 3: T-Tests on Suspension Coils
## Deliverable 4: Design a Study Comparing the MechaCar to the Competition
## Results
## Linear Regression to Predict MPG
### Using lm(mpg ~ vehicle_length+vehicle_weight+spoiler_angle+ground_clearance+AWD,MechaCar) to get the coefficient 
![](R/linear.png)
###
![](R/Slinear.png)
## Summary Statistics on Suspension Coils
### To find P-value along with r-squared value use summary(lm(mpg ~ vehicle_length+vehicle_weight+spoiler_angle+ground_clearance+AWD,MechaCar) )
## Prediction 
### With the pr(>|t|) value is greater than 0.05, there will be no significant impact on the mpg values and we can reject the null hypothesis. The linear model does not predict mpg of MechaCar prototypes effectively because the p value of the multiple linear regression is significantly higher than 0.05 there will be no significant difference
![](R/Total.png)
###
![](R/Lot.png)
## T-Tests on Suspension Coils
### For T_test1, the p value is 1.568e-11 which is greater than 0.05 and is therfore not significant and the null hypothesis can be accepted.
![](R/test1.png)
### For T_test2 , the p value is 0.0005911 which is less than 0.05 and is therfore significant so the null hypothesis can be rejected.
![](R/test2.png)
### For T_test3, the p value is 0.1589 which is greater than 0.05 and is therfore not significant so the null hypothesis can be accepted
![](R/test3.png)
## Study Design: MechaCar vs Competition
### What Metric are we going to test?
We can test the highway fuel efficiency,horse power and cost because those metrics are directly proportional we can justify the cost of vehicle comparing to the competition.
### What is the null hypothesis or alternative hypothesis?
The null hypothesis means there are no difference between a sample mean or proportion and a population mean or proportion. The alternative hypothesis is a opposite to the null hypothesis. Using the t test we can calculate the p value and depending on this p value we can reject our null hypothesis if p value is smaller than 0.05 and support the alternative hypothesis or accept the null hypothesis and reject the alternative hypothesis.
### What statistical test would you use to test the hypothesis? And why?
I would use the two sample t test because we are comparing two populations instead of using the one sample t test, which only covers one population.
### What data is needed to run the statistical test?
Means of both sample, the standard deviation of both samples, along with the number of observations are the data we need to run a statistical test.
