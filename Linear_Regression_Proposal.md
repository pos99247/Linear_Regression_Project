# House price prediction model


### Question/Need ###
---
In this project I will be trying to predict the price of houses in San Diego.  
Potential buyers will be able to get fair price of their houses instead of overpaying.

### Data Description ###
---
Data will be scraped from realtor.com.  
Every listing from the city of San Diego will be scraped from realtor.com.  
Each listing will contain the following features: Type of housing, location, square footage, property age, garage/parking, HOW fee, and etc.  
Provided with the features the model will predict a estimated price of the house.

### Tools ###
---
Webscraping will be done by using Beautiful Soup and Selenium.  
Data manipulation will be done by using Pandas and Numpy.  
Data visualizaiton will be done by using matplotlib and seaborn.  
Mapping of San Diego will be done by using Pandas(geopandas).  

### MVP Goal ###
---
All data will be cleaned with Pandas and the data will be used to model a linear regression through sklearn. When features are inputed the model should return a estimated price of the house.