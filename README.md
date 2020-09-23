# Recommender-content-based
A content based recommendation system in python 

dataset @ https://www.kaggle.com/ruchi798/movies-on-netflix-prime-video-hulu-and-disney

A simple ratings based recommender was too naive to be used at all for Friday nights, so for a resonable improvement how about we will merge all textual columns of the dataset into a single column then use a tokenizer and a TF-IDF Vectorizer to create a sparse matrix of the TF-IDF score of all words. Then we will select and normalize the numerical variables to (0,1) and add them into the sparse matrix. We will be performing the following steps for preprocessing:

*Selecting all object data types and storing them in a list.
*Removing ID and Title column.
*Joining all text/object columns using commas into a single column.
*Creating a tokenizer to remove unwanted elements from our data like symbols and numbers.
*Making a TfidfVector from the text.
*Selecting numerical variables into a data Frame.
*Normalizing the numerical variables using a minmax scaler in the range of (0,1).
*Adding numerical variables into the TF-IDF vectors sparse matrix using the hstack function (hstack is used to add horizontal arrays into a sparse matrix).
