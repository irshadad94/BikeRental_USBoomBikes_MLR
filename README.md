# BIKE SHARING - LINEAR REGRESSION MODELLING
> Multiple linear regression model for the prediction of demand for shared bikes.  


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**BACKGROUND**

A US bike-sharing provider **BoomBikes** is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

**PROBLEM STATEMENT**

BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

**OBJECTIVE**

To understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

**BUSINESS GOAL**

To model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used

- scikit-learn - version 1.5.2
- matplotlib - version  3.9.2
- pandas - version 2.2.2
- numpy - version 2.0.0
- seaborn - version 0.13.2
- statsmodels - version 0.14.4

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

**EDA Results**
- The total rent has high correlation with year as we could see year on year it is increasing. But we could no or weak correlation between weekday, workingday and holiday against total rent
- There are negative correlations between cnt with hum and windspeed.
- Temperature, humidity, and windspeed can influence bike rentals to some extent
- The weather conditions play a significant role in bike rental patterns, with clear weather and warmer temperatures being the most favorable for rentals.
- People tend to rent bikes more frequently on working days, possibly for commuting or leisure activities.
- Compared to 2018, 2019 has increased in bike rental bookings in all weather conditions. However, total rent is depending on the weather conditions. High marking of total sales in clear weather followed by mist LightSnow marks the very less total rent.
- There is heavy concentration of total rents when the windspeed is lower (7-16). If the windspeed is increasing, the total rent is tend to decrease.

**MODEL CONCLUSION**

We can see that the equation of our best fitted line is:

$ cnt = -0.5876 + 1.0489  \times  yr + 0.2514  \times  workingday + 0.4385 \times temp - 0.4727 \times seasonspring + 0.2946 \times seasonwinter +  0.1953 \times mnth5 + 0.3542 \times mnth9 + 0.2917 \times weekday6 - 1.3568 \times weathersitLightSnow - 0.3607 \times weathersitMist $

From this best fit line with minimal errors, we can interpolate the data to predict. The model came up with 81% of R2 score which denotes the model as best fit. About 81% of the variance in the target variable can be explained by the other independent variables in our model. Thus r2_score suggest a strong model fit


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- This case study is to apply multiple linear regression model for the prediction of demand for shared bikes in US Boombikes.  
- It is faciliated by IIIT - Bangalore through the AI/ML program through UpGrad
- This project was based on Linear Regression (Machine Learning)


## Contact
Created by [@irshadad94] - feel free to contact me!