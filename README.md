# Project Objective

The goal of this project is to develop an NLP model capable of predicting the daily closing
values of a stock market index based on news text. In summary, with the NLP techniques
you have learned during class, you must implement a binary classifier that, for each day,
receives news headlines and is able to predict if the index closing value rose (1) or
decreased (0).

# Corpora

Train (1690 lines):
The first column is “Id”, the unique identifier of each line/day. The second is "Closing Status" (this should be the dependent variable). This column takes the value “1” when the index closing value
rose or stayed the same; and “0” when the closing value decreased. The following columns are
news headlines ranging from "Headline1" to "Headline25”. For each line, you should use these
columns’ text (you are not required to use all columns) to predict the “Closing Status”.
Test (299 lines):
The structure of these dataset is the same as the train set, except that it does not contain the “Closing Status” column. You are expected to provide the predicted status (“1” or “0”) for each line in this set and I will compare your predictions with the actual (true) labels.

# Methodology and Conclusion
- The performance of MLP is tested for both TF-IDF vectores and Word2Vec embedding using Google News corpus
- We conclude that performance of MLP with hidden layers (25, 10) on TF-IDF performs fairly well, given the size of the dataset we have, with an accuracy of 55% and a Balanced Precision of 61%
- We also reduce dimensionality using LSA (Latent Semantic Analysis), a technique in natural language processing (NLP) and information retrieval used to discover hidden (latent) relationships between words and concepts within a large body of text. The core idea behind LSA is to reduce the dimensionality of textual data while preserving its semantic structure, which helps in understanding the meaning and usage of words and their relationships to one another.
