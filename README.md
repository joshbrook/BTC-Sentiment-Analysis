# Bitcoin Price Fluxuation Analysis based on Sentiment Analysis of Related Tweets
##### A collaboration for Text Mining by Josh Brook, Philip Ngare, and Iacob Postavaru
-------------------------------------------------------------------------

## Abstract
This project implements sentiment analysis techniques on large datasets of tweets related to Bitcoin (BTC) in order to create a model that can tag raw data with sentiments and analyse the relationship between Price and Sentiment. We aim to study correlation between the price fluxuation of cryptocurrencies and people's sentiments about them, since they are based on intangible services and as such could be considered volatile based on the availability of these services. 

We have taken a sentiment-tagged dataset of BTC-related tweets, and used that to train a machine learning model in order to automatically sentiment-tag a curated dataset which we have scraped from the Twitter API. We then compare the change in sentiment per day to the change in price of BTC per day, and employ correlation analysis in order to determine whether online sentiment influences BTC price or vice versa.


### Keywords 
Bitcoin, sentiment analysis, machine learning, natural language processing


## Research Question
Is the sentiment of online discourse about Bitcoin representative of the change in its market price? 

If there is a correlation, is there causation in either direction?


## Data
We make use of the following [Bitcoin Sentiments](https://www.kaggle.com/code/alexandrayuliu/bitcoin-tweets-sentiment-analysis/data?select=Bitcoin_tweets.csv) Dataset, containing 1.5 million sentiment tagged tweets related to Bitcoin.
- This will be useful for creating our sentiment analysis models as it has labelled data that can be used to train a model which we can later apply to unlabelled data in order to improve our model.

We have created our own dataset of Bitcoin-related discourse by using the [Twitter API](https://developer.twitter.com/en/docs/twitter-api) to pull relevant tweets from the week of the 17th to 23rd of May, which can be seen in a compressed csv file [here](data/Btc_tweets_17_23.zip). We also gained access to a researcher version of the API, which allowed us to scrape tweets from further back in time, but was unfortunately quite limited in volume. 

We also considered using the following datasets but decided to narrow our focus to achieve better results.
- [Ethereum](https://socialgrep.com/datasets/the-reddit-ethereum-dataset)
- [Apple Stock](https://socialgrep.com/datasets/five-years-of-aapl-on-reddit)
- [Cryptocurrency](https://socialgrep.com/datasets/reddit-cryptocurrency-data-for-august-2021)
> These datasets are new and offer both comments and posts with their sentiment scores which may prove useful for improving our sentiment analysis algorithm. 


## Overview of steps taken

- Choosing suitable datasets for training, testing, and prediction
- Pre-processing of tweet data
- Web crawling for Twitter data
- Data visualization
- Applying machine learning methods to sentiment-tag tweets
- Creating word vector spaces
- Performing correlation analysis
- Finding BTC price data
- Analysing importance of the age of the data 
- Word frequency and visualization


## Further Reading
Feel free to look through our code in the various Jupyter Notebooks, starting with [Preprocessing](preprocessing.ipynb).

See our [final report](report.pdf) for our in-depth discussion and analysis of results.





