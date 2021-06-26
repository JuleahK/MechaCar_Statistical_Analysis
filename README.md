# MechaCar_Statistical_Analysis

## Overview

The scope of this project is to use statistical analysis to help an auto manufacturing team. To aid in removing the production blockage, the company has requested data on which variables can predict the mpg of the new prototype car, a summary on the PSI of the suspension coils, determine which manufacturing lots are statistically different from the mean population. 


### Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/78892035/121923976-78cc8080-cd09-11eb-86c5-e1894c13418b.png)

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 

  The analysis determined that vehicle length and ground clearance most significantly impact miles     per gallon and would return a non-random amount of variance.

- Is the slope of the linear model considered to be zero? 

  The p-value of our linear regression analysis is 5.35e-11, which is much smaller than our assumed     significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject     our null hypothesis, which means that the slope of our linear model is not zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? 

  With the R-squared value at 0.7149, or about 71%, we can adequately determine the mpg of the         prototype cars.

## Summary Statistics on Suspension Coils

The specified variance of the suspension coils is to not exceed 100 PSI. The images below reveal that the lots together meet this criterion, but when analyzed individually, we see that Lot 3 has a high variance of over 170 and does exceed the requirement.

![image](https://user-images.githubusercontent.com/78892035/121925741-37d56b80-cd0b-11eb-9cc4-61e8af64c512.png)


![image](https://user-images.githubusercontent.com/78892035/121925659-255b3200-cd0b-11eb-817f-5f1e9d0b324a.png)


## T-Tests on Suspension Coils

The t-test performed yields a p-value of 0.06 and a mean of 1498.78, suggesting that all lots are statistically similar to the population mean of 1500 PSI, as seen below. 

#### T-test for all Lots
![image](https://user-images.githubusercontent.com/78892035/121927955-a74c5a80-cd0d-11eb-846b-204b5f4260f5.png)

#### T-test for Lot 1: Is statistically similar
![image](https://user-images.githubusercontent.com/78892035/121928003-b6330d00-cd0d-11eb-9c7f-3f60fbc2f153.png)

#### T-test for Lot 2: Is statistically similar
![image](https://user-images.githubusercontent.com/78892035/121928088-cb0fa080-cd0d-11eb-9496-06ab2a9557e6.png)

#### T-test for Lot 3: Is not statistically similar
![image](https://user-images.githubusercontent.com/78892035/121928134-d8c52600-cd0d-11eb-8895-09536efd30c5.png)


## Study Design: MechaCar vs Competition

In the current project we were able to determine the effect of miles per gallon based on certain variables. We could compare the prototype car to other manufacturers’ cars based on these criteria and test which cars get the best mpg as well as which are the safest. Consumers may wish to drive the most efficient and safe car possible. We could use an ANOVA test here to determine if there was a statistical difference between the safety of the prototype car and other cars. To determine this, we would need to find additional data on overall safety ratings. These may be more limited on the prototype but would undergo the same initial testing as other manufacturers’ cars. Our hypothesis would be that the prototype car would be more safe than the other cars.
