# Mission-to-Mars
Use BeautifulSoup, Splinter, and Pandas to scrape various webpages related to Mars. The scrape would be stored on Mongodb and displayed on a webpage using Flask.

## Procedure

### scrape 
Scraping initially, was done through Jupyter Notebook. Scraping was first done on the Nasa Mars News website where we scraped the latest news and text related to Mars. The second page we scraped was the JPL Space Image website. We extracted the full-size featured image from this site. The third site to be scraped was the Space Facts website which was used to gather data regarding Earth and Mars. Finally we extracted the four Mars hemisphere full-size images from USGS Astrogeology website.

After all the data was cross-checked, we transfered the code to a Python file and created a scraping function.

### Storage (MongoDB)
Once the data was scraped, we used MongoDB to store the data. Using the scraping function, the data extracted was compiled in a dictionary and stored in a MongoDB collection titled "mars".

### Display (Flask)
An instance of Flask was created and a connection to the database was established. Using the connection, the scraped data is presented on the Flask website. The website UI was updated using Bootstrap. The python code to run the flask website and HTML for the flask website has been included in the repository.

