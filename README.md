# Nivea Web-Scraping and Sentiment Analysis

Amidst the rapid trend of buying beauty products online due to the availability of variety in one place without transport and more offers, brands need to maintain a good image in front of customers. To tackle this issue, we proposed to make a sentiment analysis model that highlights the positive and negative aspects of products that these brands can use to understand the problems of their customers and give them a better experience. For this experiment, we used web scraping tools like BeautifulSoup and Python to get more than 9000 primary data and further preprocessed and labeled them according to the needs of the project objectives before preprocessing. Decision tree algorithms are the most preferred one in many data mining applications and they are basically tree like structures where internal nodes depict the decisions and the leaf nodes represent the class labels. Overfitting is the main issue of this algorithm due to depth or noise in the dataset. Therefore its extension called Random forests is more preferred as the randomness of the model reduces the overfitting of the models and improves generalization. It is also more suitable at capturing noise than decision trees, which is important for the application of sentiment analysis where data scraping has been used. This is due to the inaccuracies that occur in user input data or system translation faults.

## Web Scraping

Amazon reviews were scraped on Google Colab, with the NVIDIA T4 Tensor Core GPU. The Application Programming Interfaces (APIs) include Requests, BeautifulSoup, and DataFrame. Requests API was used to send HTTP requests, and retrieve content from the listed URLs. In order to parse the retrieved HTML content and extract specific elements, BeautifulSoup API was used. This data was manipulated and converted into a CSV (commaseparated values) file with the DataFrame API provided by the Pandas library.

<br> The scraped data is divided into 70% training data and 30% testing data. 9289 Reviews from a total of 77 Nivea products were scraped from https://www.amazon.ae/.

## Model Execution Requirements

Upon retrieving the CSV file, further manipulations and models were implemented in Jupyter Notebooks. API’s from NLTK, and Scikit-learn were used. The NLTK API provided tools for Natural Language Processing such as stemming, lemmatization, and removal of stop words. Scikitlearn provided various functionalities for the preprocessing of data, splitting into training and testing dataframes, classification, cross-validation, and methods for model evaluation.
