# Anime Data Analysis and recommendation Project

## Project Overview

Anime has become a popular form of entertainment worldwide, with a vast array of genres and titles available. This project utilizes data analysis techniques to understand trends, preferences, and correlations among anime viewers. Additionally, it provides a recommendation system to suggest anime titles to users based on their preferences.

## Data Preprocessing

- Handled missing values
- Removed duplicates
- Standardized text fields like genre in my case. (e.g., converting text to lowercase) 
- Merged the important tables in rating.csv and anime.csv after preprocessing

## Analysis

- EDA to understand the distribution of features, correlations, and trends.
- Statistical analysis like analyzing User rating trends in the rating dataset.
- Visualization techniques such as histograms and scatter plots to illustrate patterns in the data.

- ### Word Cloud
We used it to Represent the most frequent genre of the anime in the dataset. Thus, as per the popularity we can get the most popular genre among people. 

## TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) vectorization is a technique commonly used in natural language processing (NLP) to convert textual data into numerical vectors. It assigns weights to terms based on their frequency in a document and their rarity across all documents. 

- We utilized tf-idf vectorizer to convert the textual data (here anime genres) into numerical vectors.
- Each genre list is split into individual words or tokens.
- Here Using TF we measured how frequently a term (genre) occurs in a document (anime) while IDF measured the importance of a genre across the entire dataset.
- At last TF-IDF is obtained by multiplying the TF value by the IDF value for each term in the document.

## Cosine Similarity

Cosine similarity is computed between all pairs of anime based on their TF-IDF representations. <br>
So at last we measured the cosine of the angle between the two vectors that ranges from -1 to 1, with higher values indicating greater similarity.

  
