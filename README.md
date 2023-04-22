# CA2_ProgrammingForDataAnalysis

Primary objective: To design and develop a Data Acquisition, Pre-processing and Data Analysis Pipeline.

Details of assignment brief: You are required to develop a Data Acquisition, Pre-processing and Data Analysis Pipeline of your choice, including data acquisition (API, Web scraping, DB Extract etc.), Extraction of features and Transformations as appropriate, followed by loading into an appropriate database. Finally, data analysis should be done which involves answering questions of (public or self) interest based on the data. The focus of the complexity of the pipeline is your choice. Python must be used for the assignment.

# MOVIE RATING ANALYSIS

This project demonstrates how to scrape data from the website using Python's Beautiful Soup and Requests libraries, store the data in MongoDB and load as a DataFrame from MongoDB, and then analyze the data in Google Colab using Pandas. 

Getting Started

To get started, you will need to have Python 3.x installed on your machine or Google Colab. You will also need to install the following libraries:

beautifulsoup4

requests

pandas

pymongo

With the help of this Python script, you can collect information about movies from the IMDb website "https://www.imdb.com/search/title/?user_rating=6.9,10.0&adult=include&count=250" and save it in a MongoDB database. The script makes HTTP calls to the IMDb website using the requests library, then parses the HTML return using the BeautifulSoup library. Specific data is extracted using the BeautifulSoup library, including the title, year of release, IMDb rating, IMDb vote total, genre, cast members, and movie description. The pandas library, a potent data manipulation library for Python, is then used to process the scraped data.

# Data Acquisition

Scraping the Data

To scrape the data from IMDB website and run the .ipynb script. This script will use the Requests library to make a GET request to the website, and then parse the HTML using Beautiful Soup to extract the desired data. The data will then be stored in MongoDB as a DataFrame using the pymongo library. The script is made to save the data that has been scraped in a document-oriented NoSQL database called MongoDB. The information is kept in a collection called "movies" that can be easily accessed using the querying language of MongoDB. The script communicates with the MongoDB database using the PyMongo module.

Store & Load Data using MongoDB

The basic URL for the IMDb website and the HTTP request headers are defined at the beginning of the script. The movie links on the page are then extracted by sending a request to the website using the requests library and parsing the result with BeautifulSoup. The script makes a new request for each movie link and uses BeautifulSoup to retrieve the pertinent information. The data is subsequently transformed into a pandas DataFrame, allowing for simple data processing and manipulation.

# Data pre-processing

Removal of Unwanted Columns

Column Renaming

Data type conversion

Null value handling

# Data Analysis

To analyze the data, you can use Google Colab. First, need to load the data from MongoDB into Colab and once the data get loaded, it is possible to perform any necessary data analysis using pandas or other Python libraries. Following data processing, the script connects to a MongoDB database using the PyMongo module and inserts the data into the "movies" collection. The script prints out the number of records that were successfully inserted into the database and ensures that duplicate records are not added to the database.

In conclusion, this Python script shows how to use Python modules like requests, BeautifulSoup, pandas, and PyMongo to quickly scrape and store movie data from the IMDb website. It exemplifies Python's versatility and strength for data processing and web scraping jobs. The script is easily expandable to include more data fields and to scrape information from other websites.
