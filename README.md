# CA2_ProgrammingForDataAnalysis

Primary objective: To design and develop a Data Acquisition, Pre-processing and Data Analysis Pipeline.

Details of assignment brief: You are required to develop a Data Acquisition, Pre-processing and Data Analysis Pipeline of your choice, including data acquisition (API, Web scraping, DB Extract etc.), Extraction of features and Transformations as appropriate, followed by loading into an appropriate database. Finally, data analysis should be done which involves answering questions of (public or self) interest based on the data. The focus of the complexity of the pipeline is your choice. Python must be used for the assignment.

Getting Started

This project demonstrates how to scrape data from the website using Python's Beautiful Soup and Requests libraries, store the data in MongoDB and load as a DataFrame from MongoDB, and then analyze the data in Google Colab using Pandas. 

To get started, you will need to have Python 3.x installed on your machine or Google Colab. You will also need to install the following libraries:

beautifulsoup4
requests
pandas
pymongo

Scraping the Data
To scrape the data from IMDB website we are using the url "https://www.imdb.com/search/title/?user_rating=6.9,10.0&adult=include&count=250" run the .ipynb script. This script will use the Requests library to make a GET request to the website, and then parse the HTML using Beautiful Soup to extract the desired data. The data will then be stored in MongoDB as a DataFrame using the pymongo library.

Analyzing the Data
To analyze the data, you can use Google Colab. First, need to load the data from MongoDB into Colab and once the data get loaded, it is possible to perform any necessary data analysis using pandas or other Python libraries.
