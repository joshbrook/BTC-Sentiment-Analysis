# Bitcoin Price Prediction based on Sentiment Analysis of Relevant Tweets
-------------------------------------------------------------------------

## Abstract
This project employs sentiment analysis on tweets related to cryptocurrencies in order to create a model that can predict how valuations might change based on public sentiment. We decided to do this to see whether there is a correlation between the behaviour of cryptocurrencies and people's sentiments about them since they are based on intangible services and as such could be considered volatile based on the availability of these services. 

We have taken a sentiment-tagged dataset of Bitcoin ($BTC) related tweets, and used that to train a machine learning model in order to sentiment-tag a curated dataset which we have pulled from the Twitter API. We then compare the change in sentiment per day to the change in price of BTC per day, in order to analyse the correlation. Finally, we attempt to determine whether the sentiment influences the price or vice versa.


## Research questions
Is the sentiment of online discourse about Bitcoin representative of the change of its market price? If there is a correlation, which one affects the other more?


## Datasets
We will make use of the following [Bitcoin Sentiments](https://www.kaggle.com/code/alexandrayuliu/bitcoin-tweets-sentiment-analysis/data?select=Bitcoin_tweets.csv) Dataset, containing 1.5 million sentiment tagged tweets related to Bitcoin.
- This will be useful for creating our sentiment analysis models as it has labelled data that can be used to train a model which we can later apply to unlabelled data in order to improve our model.

We have created our own dataset of Bitcoin-related discourse by using the [Twitter API](https://developer.twitter.com/en/docs/twitter-api) to pull relevant tweets from the week of the 17th to 23rd of May, which can be seen in a compressed csv file [here](data/Btc_tweets_17_23.zip).

We also considered using the following datasets but decided to narrow our focus to achieve better results.
- [Ethereum](https://socialgrep.com/datasets/the-reddit-ethereum-dataset)
- [Apple Stock](https://socialgrep.com/datasets/five-years-of-aapl-on-reddit)
- [Cryptocurrency](https://socialgrep.com/datasets/reddit-cryptocurrency-data-for-august-2021). 
> These datasets are new and offer both comments and posts with their sentiment scores which may prove useful for their sentiment analysis. 


### Week one 
----------

- **Data selection**
  - Since we opted to use labelled and unlabelled datasets, we first had to find a sizeable raw dataset which we could use to further train our sentiment analysis model as well as a prediction model.
  -  For this, we found the Twitter [Bitcoin Sentiments](https://www.kaggle.com/code/alexandrayuliu/bitcoin-tweets-sentiment-analysis/data?select=Bitcoin_tweets.csv).

  
- **Pre-processing**
  - For the pre-processing, we expected to be able to display a sample of the data in order to confirm that we were able to access the raw data from twitter's Apis’ correctly.
  - This data will not include the following as they were deemed unnecessary for our analysis:
    - URLs
    - Twitter-specific URLs
    - Emojis
    - Emoticons.

### Week two
------------

**Modelling Data**
- After we pre-processed and collected all the data necessary for our analysis, we now build some models in order to predict sentiments. The Models are trained and evaluated on the Aforementioned datasets. 
-To check whether there is any correlation between price and sentiment, we apply our model to unlabelled Web Scraped raw data from the past week. 


## Roles and Divisions

### Philip
--------

- Picking datasets for training testing and prediction
- Pre-processing 
- Web crawling
- Data Visualization

### Josh
------
- Pre-processing 
- Applying machine learning methods to make predictions
- Creating word vector spaces if needed
- Performing correlation Analysis

### Iacob
--------
- Finding Bitcoin Price Data
- Choosing suitable datasets
- Analysing the importance of the age of the data 
- Pre-processing, especially cleaning the data
- Word frequency and its visualization

--------

## Documentation
***This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.***



