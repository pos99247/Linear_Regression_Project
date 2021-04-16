# Predicting Housing Prices in San Diego

---

Brian Nam

## Abstract

---

The goal of this project is to use linear regression models to predict the housing prices in San Diego. The data set was web scraped from realtor.com and San Diego Superior Court web site. The data scraped was cleaned using various exploratory data analysis techniques and domain knowledge of houses. Ridge regression model was chosen by comparing R squared scores. The model was used to predict the houses in the test set.

## Design

---

As I am currently in the market for a apartment, being able to predict a housing price with key points such as size and location seemed very useful. By accurately predicting house prices, people will not have to over pay for  houses.

## Data

---

The dataset contains 8455 sold house listings from 4/7/21 to 10/12/20 with 16 features each. The main features are bed, bath, square footage of the house, address, sold date, built year, renovated year, lot size, story, and garage. The target variable is the price each house was sold. Address, garage, and property type were transformed into categorical data using the dummy variable method.

## Algorithms

---

**Feature Engineering**
1. Using the zipcode in the address, created new columns to show whether the listing is from a expensive, average, or cheap neighborhood. The three categories were differentiated by percentile of price in the entire data.
2. Categorical data were converted into binary dummy variables.  

**Models**
Simple linear regression was used for initial modeling. After trying ridge, lasso, and polynomial in all combinations, linear ridge regression was chosen as the model due to its best performance in R squared score.

**Model Evaluation**
The entire data set was split into 8:2 = Train:test, then the valid scores were calculated with 5-fold cross validation on the training set. Then the regression was refitted with the entire set then was used to predict the test set.  
Ridge train R squared : 0.618  
Ridge cross validation R squared : 0.607  
Ridge test R squared : 0.598  
Mean Absolute Error : $206,732.73  

## Tools

---

* Beautiful Soup and Zyte for webscraping
* Pandas and numpy for data manipulation
* Seaborn and matplotlib for data visualization

## Communication

---

Slides were made for the presentation to give a better understanding of the model.