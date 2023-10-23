## Predicting House Prices in Mexico

This Folder has 2 files; both of them make Web Scrapping and Linear Regression for the house prices, but one is an automated program that uses selenium to perform web scraping on a website depending on the city that is in a txt.

**These programs are introductory to perform data analysis and web scraping. Thus we can see the principles of how to get data from the web and turn it into valuable information.**


### First Program (PricesPrediction)

 The [first program](/PricesPrediction.ipynb) reads the URL of the website that offeers houses in Mexico City, then does Web Scrapping to fetch all the data, does data cleaning, and finally does statistics calculus to obtain the linear regression, the plot and the prediction. 

### Second Program (AutomatizedPrediction)

 The [second program](AutomatizedPrediction.ipynb) does exactly the same as the first, but the difference is that at the beginning reads a txt file where you can put any city of and the program will make a prediction in that city, then uses Selenium to get the URL of the website with the offers of houses in that city and finally does the regression. 

 **Requisites for the Second Program**

- Have the lastest version of Google Chrome and Google Chrome Driver 
- Have the google chrome driver downloaded