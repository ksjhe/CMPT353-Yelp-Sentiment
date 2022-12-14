## Sentiment analysis using Recurrent Neural Network on Yelp restaurant reviews.
CMPT 353 - for Dr. Greg Baker, School of Computing Science, Simon Fraser University.

## The project
We are doing a data analysis and machine learning project for restaurants in Edmonton, AB.
The dataset for training of the RNN comes from Yelp reviews, we cleaned, organized the data and fed it through a neural network.
The machine then labels each review within the data to give users an understanding of the sentiment response of previous visitors.

## Project Report
The project report link is here. 

## Interactive Map of Positive Scores
We grouped by the dataset and visualized the data using looker studio

The first one is more a sanity check, we groupedby the data and averaged using the scores given by users for a restaurant:\
[map of edmonton with average score given by users](https://datastudio.google.com/s/q-1s3WAWPrs)

These are scores from our models, we also groupedby the data and average the positive sentiment score per restaurant:\
[map of edmonton restaurants with sentiment scores using RoBERTA](https://datastudio.google.com/s/qQ1zFA7x7r4)\
[map of edmonton restaurants with sentiment scores using VADER](https://datastudio.google.com/s/gTHQGWbg2Pg)

## Datasets:
The cleaned/trained dataset are [here](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/tree/main/data/trained) The vader model has both test and train sets.\
The roberta model includes 70% of the data, which scores are added per review.

The Edmonton only dataset without any cleaning/training can be found [here](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/tree/main/data).

Note: You can use Pandas or Spark to view dataframe. See on how to install Pandas or Spark on your local computer/cluster.\
link to install pandas API [here](https://www.pythoncentral.io/how-to-install-pandas-in-python/)\
link to install spark [here](https://medium.com/tinghaochen/how-to-install-pyspark-locally-94501eefe421)

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

install using pip or anaconda3


## Table of Contents
0. [Data Refactoring](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/0.Data%20Refactor.ipynb)
1. [Data Exploration](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/1.Explore.ipynb)
2. [Data Cleaning](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/2.Clean.ipynb)
3. [Exploratory Data Analysis](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/3.%20Exploratory%20Data%20Analysis.ipynb)
4. a) [Sentiment Modeling (Feature Engineering)](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/4a.%20Sentiment%20Modeling%20(Feature%20Engineering).ipynb)	<br> b)[ Sentiment Modeling (Researched Models)]( https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/4b.%20Sentiment%20Modeling%20(Researched%20Models).ipynb)
5. [Results/Analysis](https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/5.Analysis.ipynb)

## Graphs 

### Word Density Analysis
The data was ran on the nltk library and stopwords were removed, we wanted what words were important in the actual reviews.

<p align="center"><img src="https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/visuals/WDA.svg" width="480"></p>

### N-Gram Analysis
An N-gram checks contiguous series of words in the reviews and groups them. We wanted to see some of the more important factors on top of food quality in our dataset. 

<p align="center"><img src="https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/visuals/Ngram_Analysis.svg" width="480"></p>

Location and service seems to be a detrimental part of most of the reviews in the dataset.


### Classification Graphs
We wanted to see how our data correlates with the scores given by our two pretrained models: RoBERTa and VADER.

### VADER MODEL

<p align="center"><img src="https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/visuals/vader_test.svg" width="750"></p>

### RoBERTa MODEL

<p align="center"><img src="https://github.com/ksjhe/CMPT353-Yelp-Sentiment/blob/main/visuals/roberta.svg" width="750"></p>
