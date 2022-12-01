# CMPT353-Yelp-Sentiment


## Sentiment analysis using Recurrent Neural Network on Yelp restaurant reviews.

## The project
We are doing a data analysis and machine learning project for restaurants in Edmonton, AB.
The dataset for training of the RNN comes from Yelp reviews, we cleaned, organized the data and fed it through a neural network.
The machine then labels each review within the data to give users an understanding of the sentiment response of previous visitors.

## Interactive Map of Positive Scores
We grouped by the dataset and visualized the data using looker studio

The first one is more a sanity check, we groupedby the data and averaged using the scores given by users for a restaurant:
[map of edmonton with average score given by users](https://datastudio.google.com/s/q-1s3WAWPrs)

These are scores from our models, we also groupedby the data and average the positive sentiment score per restaurant:
[map of edmonton with positively rated restaurants using RoBERTA](https://datastudio.google.com/s/qQ1zFA7x7r4)
\n [map of edmonton with positively rated restaurants using VADER](https://datastudio.google.com/s/gTHQGWbg2Pg)


## Languages used:
Python is used including machine learning libraries and data science tools such as Pandas and numpy.
We used jupyter notebook for easier explanation and exploration of the data.
The file is then converted to a parquet file for easier storage and manipulation of data.

## Libraries Used:
Please install the following libraries:
Pytorch,
tqdm,
seaborn,
pandas,
numpy,
matplotlib,
tensorflow,
nltk

## Table of Contents
0. [Data Refactoring](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/0.Data%20Refactor.ipynb)
1. [Data Exploration](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/1.Explore.ipynb)
2. [Data Cleaning](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/2.Clean.ipynb)
3. [Exploratory Data Analysis](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/3.%20Exploratory%20Data%20Analysis.ipynb)
4. a) [Sentiment Modeling (Feature Engineering)](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/4a.%20Sentiment%20Modeling%20(Feature%20Engineering).ipynb)	<br> b)[ Sentiment Modeling (Researched Models)]( https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/4b.%20Sentiment%20Modeling%20(Researched%20Models).ipynb)
5. [Results/Analysis] ( https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/5.Analysis.ipynb)


