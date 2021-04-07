# Air bnb price prediction model


### Question/Need ###
---
In this project I will be trying to predict the price of the air bnb in San Diego.  
Consumers will be able to get fair price of their air bnb instead of overpaying.

### Data Description ###
---
Data will be scraped from airbnb.com.  
Every listing from the city of San Diego will be scraped from airbnb.com.  
Each listing will contain the following features: Type of housing, location, # of guests, various amenities, rating, reviews, weekend/weekday.
Provided with the features the model will predict a estimated price of the airbnb.

### Tools ###
---
Webscraping will be done by using Beautiful Soup and Selenium.  
Data manipulation will be done by using Pandas and Numpy.
Data visualizaiton will be done by using matplotlib and seaborn.  
Mapping of San Diego will be done by using Pandas(geopandas).  

### MVP Goal ###
---
All data will be cleaned with Pandas and the data will be used to model a linear regression through sklearn. When features are inputed the model should return a estimated price of the air bnb.