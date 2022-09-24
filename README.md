# MechaCar_Statistical_Analysis
Used variety of statistical tests and hypothesis testing (R) to analyze series of datasets from the automotive industry (AutosRUs)

## Overview of Project
R is a programming language that has a variety of uses in data science. R has solidified itself in academia and industry as one of the go-to programming languages for statistical modelling and hypothesis testing. Our analysis include visualizations, statistical tests, and interpretation of the results. All of our statistical analysis and visualizations will be written in the R programming language. We extracted, transformed, and loaded (ETL) data; visualized the data; and analyzed the data using R. For this project, our goal is to review the company AutosRUs' newest prototype, the MechaCar's, production data for ingights that may help the manufacturing team. 

## Linear Regression to Predict MPG

<img width="800" alt="linear_regression_summary" src="https://user-images.githubusercontent.com/107021231/192070116-3c282d8b-1f34-49eb-add0-22c10da523bf.png">

* Variance of a non-random variable is usually 0. From the *Linear Regression Summary* data, the *intercept*, *vehicle_length*, and *ground_clearance* coefficients provide a non-random amount of variance to hte mpg values.  

* Assuming significance level of 0.05, the p-value is smaller, so we are able to reject the null hypothesis. The null hypothesis of a linear regression states that the slope (β1) is equal to 0. As a result, if we reject the null hypothesis, we're stating that the alternate hypothesis is true; the slope is not 0. 

* Multiple R-squared increases as more variables pass through the regression. However, adjusted R-squared controls agaisnt this increase, and adds penalities for the number of predictors in the model, therefore making it a more accurate predictor of how effective the linear model is. According to the *Linear Regression Summary* data, an *Adjusted R-squared* value of 0.6825 reveals that this linear model predict the mpg of MechaCar prototpyes effectively (relatively well). 


## Summary Statistics on Suspension Coils 

<p align="center">
<img width="400" alt="total_summary_table" src="https://user-images.githubusercontent.com/107021231/192070156-60080b44-67d7-4d1b-8be5-0ec582affc8d.png">
  
<p align="center">
<img width="400" alt="lot_summary_table" src="https://user-images.githubusercontent.com/107021231/192070164-505a1049-4c18-43bd-8e44-842eee490657.png">



* Which variables


## T-Tests on Suspension Coils

* Which variables


## Study Design: MechaCar vs Competition

* Which variables


