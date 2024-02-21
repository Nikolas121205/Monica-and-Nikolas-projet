# Exploratory Data Analysis (Statistical Programming Exercise)


# CANVA PRESENTATION:

https://www.canva.com/design/DAF9c0mTDVo/DyIDLjrwWQpJL0BKiT-0UA/edit



## 1. Introduction
This repository contains a Python script for performing exploratory data analysis (EDA) on a dataset of orders coming from Fake partners in an app. Fake partners are stores not directly integrated with the delivery app, so the content team manages their product catalog and prices. The dataset includes information such as order ID, activation time, country code, store address, final status, payment status, products, products total, and purchase total price.


## 2. Data Analysis
The script reads the dataset from a CSV file and renames the columns for better readability. It then defines a function to compare the products total with the purchase total price and assigns an authorization status to each order based on this comparison.

### Question 1: What percent of orders are under-authorized?
First, we calculate the percentage of under-authorized orders and plots a pie chart to visualize the distribution of under-authorized and authorized orders.

PIE CHAR  - PLOT 1

The percentage of orders that are under-authorized is: 57.58%


### Question 2: What percent of orders would be correctly authorized w/ incremental authorisation?
This time, we calculate the percentage of orders that would be correctly authorized with incremental authorization (20% increase in products total) and also plots a pie chart to visualize the distribution of authorized and under-authorized orders.


PIE CHAR  - PLOT 2


Now, the percentage of orders that are under authorized is: 69.03%. The under authorized orders rise approximately 12%


#### Question 3: Are there differences when split by country?

We have created a subset of under-authorized orders, groups them by country code, and calculates the percentage of under-authorized orders for each country. 

For simplifying the plot, we grouped all countries representing less than 2% of under-authorized orders into a group called "Others" 

We’ve plot the results with a  pie chart.


SAY SOMETHING ABOUT COUNTRIES 


## 3. Results --CHANGE 
The script will print the percentage of under-authorized orders, the percentage of orders that would be correctly authorized with incremental authorization, and display pie charts showing the distribution of under-authorized and authorized orders and the distribution of under-authorized orders by country.


## 4. Conclusion
This EDA provides insights into the authorization status of orders from Fake partners and the potential impact of incremental authorization. Further analysis and modeling can be performed to understand the price fluctuation of past orders and assess the risk of moving to an authorize-and-capture model.

