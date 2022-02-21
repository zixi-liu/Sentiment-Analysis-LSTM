# Sentiment-Analysis-LSTM

**Note:** the main branch contains jupyter notebook to implement Long short-term memory (LSTM) architecture for sentiment analysis on IMDB Movie Review.

***

<img src="https://github.com/zixi-liu/Sentiment-Analysis-LSTM/blob/main/img/LSTM-Backbone.png" alt="LSTM"/>

 <br />
  
## Data Source

The modeling dataset, **movie_review_data.tsv**, has 35,000 rows and 4 columns:
- Col 1: id, the identification number.
- Col 2: sentiment, 0 = negative and 1 = positive.
- Col 3: score, the 10-point score assigned by the reviewer. Scores 1-4 correspond to negative sentiment; Scores 7-10 correspond to positive sentiment. This dataset contains
no reviews with score 5 or 6.
- Col 4: review.

The score dataset, **score_data.tsv**, has 15,000 rows and 2 columns:
- Col 1: id, the identification number.
- Col 2: review.

## Methods

Since the task is a binary classification problem, the procedures to approach the problem are as follows:

- Preprocessed the review texts by cleaning, normalizing and tokenizing (segmenting) texts to prepare for the text corpus;
- Trained a standlone vocabulary list (less than 1000 rows) from word embedding base on the corpus using word2vec;
- Built a sentiment analysis model based on Long short-term memory Netwok (LSTM), which is a Recurrent Neural Network (RNN) based model, in order to try to predict if an review is positive (1) or negative (0); Word embedding and sentiment are then fed into the LSTM model and train over cycles.
- The classification performance was evaluated using the area under the ROC curve (AUC). Confusion matrix from the best performing model and performance improvement over training cycles are demonstrated.
