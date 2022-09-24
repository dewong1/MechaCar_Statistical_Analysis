# MechaCar_Statistical_Analysis
Used variety of statistical tests and hypothesis testing (R) to analyze series of datasets from the automotive industry (AutosRUs)

## Overview of Project
R is a programming language that has a variety of uses in data science. R has solidified itself in academia and industry as one of the go-to programming languages for statistical modelling and hypothesis testing. Our analysis include visualizations, statistical tests, and interpretation of the results. All of our statistical analysis and visualizations will be written in the R programming language. We extracted, transformed, and loaded (ETL) data; visualized the data; and analyzed the data using R. For this project, our goal is to review the company AutosRUs' newest prototype, the MechaCar's, production data for ingights that may help the manufacturing team. 

## Linear Regression to Predict MPG

<img width="900" alt="linear_regression_summary" src="https://user-images.githubusercontent.com/107021231/192070116-3c282d8b-1f34-49eb-add0-22c10da523bf.png">

* Variance of a non-random variable is usually 0. From the *Linear Regression Summary* data, the *intercept*, *vehicle_length*, and *ground_clearance* coefficients provide a non-random amount of variance to the mpg values.  

* Assuming significance level of 0.05, the p-value is smaller (5.35e-11), so we are able to reject the null hypothesis. The null hypothesis of a linear regression states that the slope (β1) is equal to 0. As a result, if we reject the null hypothesis, we're stating that the alternate hypothesis is true; the slope is not 0. 

* Multiple R-squared increases as more variables pass through the regression. However, adjusted R-squared controls agaisnt this increase, and adds penalities for the number of predictors in the model, therefore making it a more accurate predictor of how effective the linear model is. Based on the *Linear Regression Summary* data, an *Adjusted R-squared* value of 0.6825 reveals that this linear model predict the mpg of MechaCar prototpyes effectively (relatively well). 


## Summary Statistics on Suspension Coils 

<p align="center">
<img width="400" alt="total_summary_table" src="https://user-images.githubusercontent.com/107021231/192070156-60080b44-67d7-4d1b-8be5-0ec582affc8d.png">
  
<p align="center">
<img width="400" alt="lot_summary_table" src="https://user-images.githubusercontent.com/107021231/192070164-505a1049-4c18-43bd-8e44-842eee490657.png">

Based on the *Total Summary Table* data, the overall variance (~62.29) for the entire dataset shows that the current manufacturing data meets the 100 pounds per square inch variance limitation. However, looking at the *Lot Summary Table* data, when the data is separated into three lots, it appears that Lot3 exceed the 100 pound per square inch variance limitation with a variance greater than a hundred (~170.29). Since the lots are chosen randomly, there is a possibility that a portion of the lot does not meet the necessary suspension coils requirement. 
  

## T-Tests on Suspension Coils
  
### T-Test on Entire Lot
  
<img width="600" alt="t-test" src="https://user-images.githubusercontent.com/107021231/192072595-18c3d4f2-fd7c-4fde-9758-5f1e2066aec3.png">
  
Assuming significance level at 0.05, with a greater *p-value* (~0.06), there is not enough evidence to reject the null hypothesis. As a result, we cannot reject the fact that the sample mean may be equivalent to the true population mean. In addition, the data reveals the narrow *confidence interval*. Although a narrower confidence interval suggests that there's a smaller chance of obtaining an observation within that interval, it presents greater accuracy than a wider interval. 

 
### T-Test on Three Smaller Lots
  
<img width="600" alt="lots_t-test" src="https://user-images.githubusercontent.com/107021231/192072609-4e28ca80-d9ff-418a-b49a-da2334b3b0c4.png">
  
  
  
 #### Lot 1

* At a significance level of 0.05, with a greater *p-value* (1), there is not enough evidence to reject the null hypothesis.
  
#### Lot 2

* At a significance level of 0.05, with a greater *p-value* (~0.6), there is not enough evidence to reject the null hypothesis.
  
#### Lot 3

* At a significance level of 0.05, with a smaller *p-value* (~0.4), we are able to reject the null hypothesis. The mean of this sample is significantly smaller in comparison to the previous two lots. And unlike, the previous two lots, the confidence interval for the third lot does not include the predicted population mean. 


## Study Design: MechaCar vs Competition

Another statistical study that can quantify how the MechaCar performs agaisnt its competition is a linear regression on city and highway fuel efficiency. Gas prices are becoming increasingly expensive nowadays, and probably one of the high priority concens for consumers when purchasing a car. The metrics that may include: 

* City and highway fuel efficiency (dependent variable)
* Horse power (independent variable)
* MPG (independent variable)
* AWD capabilities (independent variable)
* Vehicle weight (independent variable)


