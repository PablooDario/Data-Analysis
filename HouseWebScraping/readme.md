# Predicting House Prices in Mexico

**These programs are introductory to perform data analysis and web scraping. Thus we can see the principles of how to get data from the web and turn it into valuable information.**

## What is it about?

We started with using web scraping to **extract data** from a website that sells houses; then we do a **data cleansing**, because when we do web scraping we extract all the data contained in the page and not the data we want, therefore in the cleaning, we will **keep only what we want**. To be able to use these data in mathematical operations we made **data transformation** and finally to make the **prediction**, we will make use of simple linear regression; as we will use only 1 independent variable, we will use the **Ordinary Least Squares** *(OLS)* method and we will make its graph for a visualization of the data.

The only diference between both programs is that one is an automated program that uses selenium to perform the web scraping on a website depending what is in a txt file.

## Web Scrapping

We use web scraping as an automated method to extract large amounts of data from websites; usually these data found on websites are unstructured; so we web scraping also help us to collect that unstructured data and store it in structured form.

### How it works?

When any web scraping code is run the request is sent to the URL that you have mentioned. The website responds to the request by sending data and allows it to read the XML or HTML page. The code will then extract the required data.

## Data Cleansing and Tranformation

Data cleansing is the process of removing incorrect, corrupted, incorrectly formatted, duplicate or incomplete data within a dataset. If data is incorrect, outcomes and algorithms are unreliable, even though they may look correct. On the other hand data transformation is the process of converting data from one format, type or structure into another.

## Prediction with Linear Regression

Linear regression is used to predict the value of a variable based on the value of another variable. Linear regression fits a straight line that minimizes the discrepancies between predicted and actual output values. To have the predictions we use the following formula:

$$\Huge\hat{y}= b_0 + b_1x$$

Where $y$ is the price of the house and $x$ the size.

Since we use the ordinary least squares method we need to find the $b_0$ and $b_1$ values that minimize the sum of the squares of the deviations between the observed values of the dependent variable $y_i$ and the estimated values of the same $\^{y_i}$. In other words, we minimize the sum of the residuals or the error. So the formula for $b_0$ and $b_1$ is:

$\Huge b_0=\frac{\sum y_i - \sum b_1x_i}{n}=\bar{y}-b_1\bar{x}$

$\Huge b_1=\frac{n\sum x_iy_i - \sum x_i \sum y_i}{n\sum x_i^{2}-(\sum x_i)^{2}}$

### First Program (PricesPrediction)

 The [first program](/PricesPrediction.ipynb) reads the URL of the website that offers houses in Mexico City, then does Web Scrapping to fetch all the data, does data cleaning, and finally does statistics calculus to obtain the linear regression, the plot and the prediction. 

### Second Program (AutomatizedPrediction)

 The [second program](AutomatizedPrediction.ipynb) does exactly the same as the first, but the difference is that at the beginning reads a txt file where you can put any city of and the program will make a prediction in that city, then uses Selenium to get the URL of the website with the offers of houses in that city and finally does the regression. 

 **Requisites for the Second Program**

- Have the lastest version of Google Chrome and Google Chrome Driver 
- Have the google chrome driver downloaded