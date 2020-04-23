# guess_the_FRIEND
FRIENDS quote prediction using FRIENDS embeddings (an Udacity Data Science Nanodegree project).

## Installation

Appart from the common Numpy and Pandas libraries, the project relies on Python 3.* and:
- [Keras](https://keras.io/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [FastText](https://fasttext.cc/docs/en/english-vectors.html) Common Crawl embeddings.

## Data

Data comes from [here](https://github.com/shilpibhattacharyya/Friends_Analysis/blob/master/friends_dataset.csv) and contains more than 90K FRIENDS lines from all 10 seasons.

## Project Overview

Starting from [this](https://fangj.github.io/friends/) data, conveniently curated and merged into a single csv file [here](https://github.com/shilpibhattacharyya/Friends_Analysis/blob/master/friends_dataset.csv), the project uses part of the lines available in the data to create an LSTM-based language model for each FRIENDS character starting from pre-traing [FastText](https://fasttext.cc/docs/en/english-vectors.html) word embeddings. With these models in hand, a classification model is then created that is able to accurately predict the friend who said a given line.

A more detailed description of the project can be found [here](https://medium.com/@alexteodor/the-one-with-the-friends-language-models-a91a7cc273c5).

## Available files

- Pre-trained language models for each FRIENDS character trained with quotes from Seasons 1-8.
- Jupyter Notebook with code for downloading the data, creating the above mentioned models and training and testing a quote classification model on data from Seasons 9 and 10.

## Instructions for running the project:

Pre-trained FRIENDS embeddings for each character are provided, but there is code available to train your own, maybe using a different architecture. Running the entire notebook will download FastText vectors, create the language models and train the quote calssifier.

## Licensing, Authors, Acknowledgements
Feel free to use the code here as you would like!
Thank you [shilpibhattacharyya](https://github.com/shilpibhattacharyya/Friends_Analysis) for making the curated data available.
