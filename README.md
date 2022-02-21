# Sentiment-Analysis-LSTM

**Note:** the main branch contains jupyter notebook to implement Long short-term memory (LSTM) architecture for sentiment analysis on IMDB Movie Review.

***

<img src="https://github.com/zixi-liu/Sentiment-Analysis-LSTM/blob/main/img/LSTM-Backbone.png" alt="LSTM"/>

 <br />
 <br />
  
## Data Source

The modeling dataset, **movie_review_data.tsv**, has 35,000 rows and 4 columns:
- Col 1: id, the identification number.
- Col 2: sentiment, 0 = negative and 1 = positive.
- Col 3: score, the 10-point score assigned by the reviewer. Scores 1-4 correspond to negative sentiment; Scores 7-10 correspond to positive sentiment. This dataset contains
no reviews with score 5 or 6.
- Col 4: review.
The score dataset, score_data.tsv, has 15,000 rows and 2 columns:
- Col 1: id, the identification number.
- Col 2: review.
