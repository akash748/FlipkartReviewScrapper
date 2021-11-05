
# Flipkart Review Scrapper

This code helps to scrap top 10 reviews from Flipkart of a user entered product.


Link : https://flipkartscrapper2700.herokuapp.com/






## Highlights

Web scraping is a technique using which the webpages from the internet are fetched and parsed to understand and extract specific information similar to a human being. Web scrapping consists of two parts:

•	Web Crawling- Accessing the webpages over the internet and pulling data from them.

•	HTML Parsing- Parsing the HTML content of the webpages obtained through web crawling and then extracting specific information from it.
Hence, web scrappers are applications/bots, which automatically send requests to websites and then extract the desired information from the website output.
Let’s take an example: 
how do we buy a phone online?
1.	We first look for a phone with good reviews
2.	We see on which website it’s available at the lowest price
3.	We check whether it’s  delivered in our area or not
4.	If everything looks good, then we buy the phone.
What if there is a computer program that can do all of these for us? That’s what web scrappers necessarily do. They try to understand the webpage content as a human would do.
Other examples of the applications of web scrapping are:
•	Competitive pricing.
•	Manufacturers monitor the market, whether the retailer is maintaining a minimum price or not.
•	Sentiment analysis of the consumers, whether they are happy with the services and products or not.
•	To aggregate news articles.
•	To aggregate Marketing data.
•	To gain financial insights from the market.
•	To gather data for research.
•	To generate marketing leads.
•	To collect trending topics by media houses.
And, the list goes on. 
In this document, we’ll take the example of buying a phone online further and try to scrap the reviews from the website about the phone that we are planning to buy.




## Installation

Download the zip folder of the project or clone it and then unzip it

Create a new virtual Environment

Install the requirements.txt file

```python
  pip install -r requirements.txt
  
```
    
## Demo

Insert gif or link to demo


## Steps Before Cloud Deployment


We need to change our code a bit so that it works unhindered on the cloud, as well.

a)	Add a file called ‘gitignore’ inside the ‘reviewScrapper’ folder. This folder contains the list of the files which we don’t want to include in the git repository. 

b) b)	Add a file called ‘Procfile’ inside the ‘reviewScrapper’ folder. This folder contains the command to run the flask application once deployed on the server:


```python
  web: gunicorn app:app
```

Here, the keyword ‘web’ specifies that the application is a web application. And the part ‘app:app’ instructs the program to look for a flask application called ‘app’ inside the ‘app.py’ file. Gunicorn is a Web Server Gateway Interface (WSGI) HTTP server for Python.



## Deployment

I have done the deployment on Heroku

a) After installing the Heroku CLI, Open a command prompt window and navigate to your ‘reviewScrapper’ folder.

b) Type the command ‘heroku login’ to login to your heroku account as shown   below:

c) After logging in to Heroku, enter the command ‘heroku create’ to create a heroku app. It will give you the URL of your Heroku app after successful creation.

d) Before deploying the code to the Heroku cloud, we need to commit the changes to the local git repository.

e) Type the command ‘git init to initialize a local git repository 

f) Enter the command ‘git status’ to see the uncommitted changes

g) Enter the command ‘git add .’ to add the uncommitted changes to the local repository.

h) Enter the command ‘git commit -am "make it better"’ to commit the changes to the local repository

i) Enter the command ‘git push heroku master’ to push the code to the heroku cloud.

j) After deployment, heroku gives you the URL to hit the web API.
