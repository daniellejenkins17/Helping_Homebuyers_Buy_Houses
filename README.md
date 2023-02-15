

# Data Science: Helping Homebuyers Purchase Fixer-Uppers

The Business Problem: 
Homebuyers in Kings County think it’s important to get the most value per dollar, when looking at houses to buy. We created a linear regression model, keeping in mind which factors might influence the price of houses.

Dataset: Kings County House Sales, 21,597 samples total, from 2014-2015 

Data Cleaning: 
We dropped irrelevant columns: date, square feet above the basement, coordinates of the location of the house, square footage of the houses for the nearest 15 neighbors, and square footage of the lots of the nearest 15 neighbors. 

![Heatmap](https://i.imgur.com/hqtbSng.png)

Baseline Model: 
We created pair plots and a heatmap of all of the values paired with each other. The features we compared against price in the initial linear regression model were: bedrooms, bathrooms,  sqft_living, sqft_lot, floors, waterfront, view, and grade. 

We took the values most highly correlated with our target variable (house price) from the heatmap, and created a baseline linear regression. The initial R-squared value was 0.62 

![Baseline Model](https://i.imgur.com/qW7Euoy.jpg)

Creating a House Price Predictor Model: 
The features that correlate most highly with house price are: 
Number of bathrooms, sqft_living, sqft_lot, waterfront, view, grade, condition, and zip code. The R-squared value for the prediction model is 0.80. These particular features help to predict the house price within 80% accuracy. 

![Sq Footage vs House Price](https://i.imgur.com/7VMJBNs.png)

![Predictor Model](https://i.imgur.com/qW7Euoy.jpg)

Recommendations Based on Coefficients of the Features:
The more bathrooms you add, the more money you lose on average. Waterfront properties increase the value of the house by $735,600 on average. When the view of the house increases by one unit, the value of the house increases by $63,000 on average. Grade and condition are highly correlated with price, so these are good metrics to use when predicting the price of a house. The square footage of the living area increases the value much more than the square footage of the lots.
