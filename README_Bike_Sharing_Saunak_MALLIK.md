# Case study/ Project: Demand for shared bikes - By Saunak MALLIK
> Description: This assignment is a Machine Learning programming assignment to build a multiple linear regression model for the prediction of demand for shared bikes.
> Note: This case study is for learning/ educational purposes only.
 
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.
- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.  
- In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits. 
- The company want to understand: the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. 
- The company wants to know: Which variables are significant in predicting the demand for shared bikes. How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors 
- A model has to be built to predict the demand for shared bikes with the available independent variables.
- The said model will be used by the management to understand how exactly the demands vary with different features.
- They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations.
- Further, the model will be a good way for management to understand the demand dynamics of a new maparation:
- "day.csv" dataset is used in this project.

## Conclusions
- Conclusion 1 : Data Pre-processing. Data defects and cleansing was performed on the initial dataset. There are no missing values. However, few features were outrightly dropped as they are not features of the data. e.g., casual, registered and instant. Some features had to be dummy encoded to fit the categorical data fit for Linear Regression.

- Conclusion 2 :  Data visualization was performed using pandas, seaborn and matplotlib libraries. Univariate, bivariate and multi-variate analysis are performed on the data set. PAirplot, Box plot, Scatter plot and Heatmap were used to perform analysis.

- Conclusion 3 :  Training and Testing data was split in the 70:30 ratio. Scaling was performed on the numerical variables. Note that hot-encoded, dummy encoded and Yes/ No, 0/1 type variables were not scaled. MinMax scaling was used.

- Conclusion 4 : A Hybrid approach to model building was adopted. Initially, sklearn.RFE method (Recursive Feature Elemination)was used to find the best-fit features. Subsequently, statsmodel.API was used to perform Linear Regression model. After modeling, feature variables were checked for p-value<0.05 and VIF<5. Variables were dropped and recursively models were built, to finally arrive at the optimum model.

- Conclusion 5 :Line of best fit for the Multiple Linear Regression Equation Model to describe the probability of renting a bike is -
   cnt =  0.2398	+ 0.2631*yr  - 0.1741*windspeed + 0.2926*spring + 0.1992*Mist + 0.2931*clear
- Conclusion 6 : The R-square of the model based on the Training dataset was found to be 73.4% while the same on the Test dataset was 71.5%. Hence, I could conclude that the model is reliable.

	- I also observed that Error terms are normally histogram of error terms they are normally distributed (bell curve).

	- I also observed thatthe error terms are independent of each other.This is evident from the scatter plot that shows the error terms are distributed about the mean.

	- I also observed that there is no observed pattern in the plot.

	- Error terms have constant variance (homoscedasticity):The variance should not increase (or decrease) as the error values change. Also, the variance should not follow any pattern as the error terms change. Univariate, Bi-Variate and Multi Variate analysis is done on the data set.

	- All these confirms the validity of the predicted model.

- Business Conclusions :  I could infer following about categorical variables –
	- mist weather conditions (Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist) has higher probability of hiring a bike
	- clear weather conditions (Clear, Few clouds, Partly cloudy, Partly cloudy) has higher probability of hiring a bike
	- In spring, there is a higher probability of hiring a bike
	- The bike rental trend is increasing year-on-year. Hence, the popularity of the bike rentals seems on an increasing trend.
   	- High bike rentals are observed in summer and fall seasons.
	- High bike rentals are observed in the months of July-Sep during the holiday seasons.



## Technologies Used
- python 3 with Jupyter Note Book
- libraries used - sklearn, statsmodels.api, numpy, pandas, warnings
- libraries used for data visualization - matplotlib, seaborn


## Acknowledgements

- This project and the data was provided by [IIITB] (https://www.iiitb.ac.in/) & [upGrad](https://www.upgrad.com/) learning platform.
- Please note that the dataset is for learning purposes only.


## Contact
- Created by [Saunak MALLIK]
(https://github.com/saunakmallik2502/)- feel free to contact me!
- Project work repository : [Demand For Shared Bikes](https://github.com/saunakmallik2502/Linear-Regression).
