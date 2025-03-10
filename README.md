# PriceOfACar
UC Berkeley AI/ML Course Assignment: What Drives the Price of a Car?

## Business Understanding

From a business perspective, we are tasked with identifying key drivers for used car prices.  In the CRISP-DM overview, we are asked to convert this business framing to a data problem definition.  Using a few sentences, reframe the task as a data task with the appropriate technical vocabulary. 

##### Understanding the Business Context

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


