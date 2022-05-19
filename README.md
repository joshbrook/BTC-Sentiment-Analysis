# Cryptocurrency prediction Based on Sentiment Analysis

## Abstract
For our project, we have chosen to use sentiment analysis on data related to cryptocurrencies and other financial derivatives to try to create a model that can predict how the financial instruments might change based on the sentiments of the public.

We decided to do this to see whether there is a correlation between the behaviour of cryptocurrencies and people's sentiments about them since they are based on intangible services and as such could be considered volite based on the availability of these services.

For this purpose, we have chosen datasets related to cryptocurrencies as well as a dataset that has Tweets that are related to Apple stock (Appl).
We hope to be able to run through a full NLP pipeline and implement machine learning algorithms, particularly ones centred on Neural Networks to showcase their superior ability in handling large data sets.

## Research questions
For our project, we have chosen to use sentiment analysis on data related to cryptocurrencies and other financial derivatives to try to create a model that can predict how the financial instruments might change based on the sentiments of the public. 

## Dataset
We will make use of the [UCC](https://github.com/conversationai/unhealthy-conversations) (The Unhealthy Comments Corpus), which contains > 40,000 online comments which have been tagged with sentiment values to train our prediction model.
- This will be useful for creating our sentiment analysis models as it has labelled data that can be used to train a model which we can later apply to unlabelled data in order to improve our model.
We will also make use of the following [Bitcoin_Sentiments](https://www.kaggle.com/code/alexandrayuliu/bitcoin-tweets-sentiment-analysis/data?select=Bitcoin_tweets.csv) Dataset that aslo features sentiment tagged Tweets related to Bitcoin tags.

We also considered using the following datasets but decided to narrow our focus to achieve better results.
- [Ethereum](https://socialgrep.com/datasets/the-reddit-ethereum-dataset)
- [Apple stock](https://socialgrep.com/datasets/five-years-of-aapl-on-reddit)
- [cryptocurrency](https://socialgrep.com/datasets/reddit-cryptocurrency-data-for-august-2021). 
>These datasets are relatively new and offer both comments and posts with their sentiment scores which will be useful for their sentiment analysis. 

## A tentative list of milestones for the project

### Week 1 
----------


- **Data selection**
  - Since we opted to use labelled and unlabelled datasets, we first had to find a sizeable raw dataset which we could use to further train our sentiment analysis model as well as a prediction model.
  -  For this, we found the Twitter[Bitcoin_Sentiments](https://www.kaggle.com/code/alexandrayuliu/bitcoin-tweets-sentiment-analysis/data?select=Bitcoin_tweets.csv).

  
- **Pre-processing**
  - For the pre-processing, we expected to be able to display a sample of the data in order to confirm that we were able to access the raw data from twitter's Apis’ correctly.
  - This data will not include the following as they were deemed unnecessary for our analysis:
    - URLs
    - Twitter-specific URLs
    - Emojis
    - Emoticons.

### Week 2
------------


**Modelling Data**
- After we pre-processed and collected all the data necessary for our analysis we now build some models inorder to predict sentiments. The Models are trained and tested on the Aforementioned datasets. 
-To check whether there is any correlation between price and sentiment, we apply our model to unlabeled Web Scrapped raw data from the past week. 

## Roles and Divisions



### Philip
--------

- Picking datasets for training testing and prediction
- Pre-processing 
- Webcrawling
- Data Visualization

### Josh
------
- Pre-processing 
- Applying machine learning methods to make predictions
- Creating word vector spaces if needed
- Word frequency distributions

### Iacob
--------
- Finding Bitcoin Price Data
- Performing correlation Analysis
- Final Report

--------

## Documentation
***This can be added as the project unfolds. You should describe, in particular, what your repo contains and how to reproduce your results.***


