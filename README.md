# PriceOfACar
UC Berkeley AI/ML Course Assignment: What Drives the Price of a Car?

## Business Understanding

The problem is to determine the most influential factors of second-hand car prices from the given dataset so that car dealers can make better decisions regarding which cars to supply in their dealerships. Knowing the variables that drive demand and price, dealers can make tactical choices on which cars to choose so that they will sell faster and at reasonable prices, hence maximizing returns.

##### Business Context

Understanding the business context is essential in determining the factors that drive used car prices. Knowing these significant attributes assists dealerships in making informed inventory choices as well as support sales teams in creating competitive pricing schemes. Knowing market trends also helps businesses in prioritizing vehicles that are in high demand and maximizing sales efforts. 

##### Defining Success

The study seeks to reveal the most significant determinants of automobile prices, providing practical guidance for pricing strategy and inventory management. With this information in hand, dealers are able to make more informed decisions that maximize profitability while being competitive in the marketplace.

Despite the massive car listings in the dataset, data preprocessing would need to be done to address missing values and outliers. This is crucial to ensure accuracy and reliability even if this would mean having a reduced sample size for developing the model.

## Data Understanding

There were unrealistic values in the dataset when it was first analyzed, such as cars with a price of zero and weird odometer readings (e.g., single-digit values). These outliers were excluded in data preparation.

Price vs. Make for Vehicles with More Than 120,000 Miles:
![image](https://github.com/user-attachments/assets/0be40b77-ae99-4531-89eb-d36008bbada5)

The graph shows significant variation in the prices of automobiles by manufacturer. As a case in point, luxury brands are observed to have pricier automobiles even when mileage exceeds 120,000 miles, while economy brands show a more significant drop in prices. This is noteworthy in ascertaining the contribution of the manufacturer to price.

## Data Preparation

##### Data Cleaning Process

Records with unrealistic price or odometer values were removed (i.e., zero price values and unrealistic mileage).
Additional Filters: Vehicles more than 10 years old were separated for the price effect analysis by age. The data was filtered further to have cars with more than 100,000 miles to ensure that the results are significant.

Price vs. Condition for Cars with More Than 100,000 Miles and More Than 10 Years Old:
![image](https://github.com/user-attachments/assets/a841011e-4857-49d8-a11e-fa1bdfdfdb53)

This graph looks at the impact of the high-mileage, older car's condition on price. The data indicated that condition was still a valid determinant of price, even in cars with over 100,000 miles and greater than 10 years old. Cars in "excellent" and "good" condition commanded the most money, and "fair" and "poor" condition were considerably less.

## Regression Models

##### Regression Analysis Summary

I tried several models, such as random forest and linear regression models, with features such as odometer reading, condition, age, and make. I tried to see if I could model car prices based on these variables.
Model Performance: Models trained on higher-mileage vehicles (i.e., 150,000-200,000 miles) were less accurate in their predictions, with greater variability in price. It was our hypothesis that the relationship between mileage and price is nonlinear and requires more advanced modeling.
Model Example: Price by Age for Cars with More Than 200,000 Miles:
The correlation between price and age for cars with more than 200,000 miles on them was not quite as strong, but there was a weak negative correlation, indicating that older high-mileage cars depreciate faster than younger cars of comparable mileage.
![image](https://github.com/user-attachments/assets/2c8a8f08-91ad-47aa-b8a7-d29abd09dc49)


