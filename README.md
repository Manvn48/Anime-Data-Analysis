# Anime Data Analysis and recommendation Project

## Project Overview

Anime has become a popular form of entertainment worldwide, with a vast array of genres and titles available. This project utilizes data analysis techniques to understand trends, preferences, and correlations among anime viewers. Additionally, it provides a recommendation system to suggest anime titles to users based on their preferences.

## Data Preprocessing

- Handled missing values
- Removed duplicates
- Standardized text fields like genre in my case. (e.g., converting text to lowercase) 
- Merged the important tables in rating.csv and anime.csv after preprocessing

## Analysis

#### EDA to understand the distribution of features, correlations, and trends.
![corr](https://github.com/Manvn48/Anime-Data-Analysis/assets/142496783/0cb468d1-de67-440c-b21a-f157bbc570b3) <br>
- Here "Members" and "avg_rating" have a positive relationship.i.e. 0.54. Because as the number of members increase avg rating of the anime will also increase. There is no Strong relationship betIen any attributes. Though "Members" and "episodes" also have corr of 0.26, as some people prefer shorter animes(like 12 to 24 episodes per season) while some prefer long(300+ episodes)

#### Statistical analysis like analyzing User rating trends in the rating dataset and applied Visualization techniques such as histograms and Pie chart to illustrate patterns in the data.
![top 10](https://github.com/Manvn48/Anime-Data-Analysis/assets/142496783/e89a8351-40a0-4773-babd-9b184660876a) <br> <br>
![Distribution of types](https://github.com/Manvn48/Anime-Data-Analysis/assets/142496783/d0813b03-d992-48c8-af3a-71c7d97da34a) <br> <br>
![sns plot for genres](https://github.com/Manvn48/Anime-Data-Analysis/assets/142496783/9eda37b2-ce1c-4fbe-92ab-d4984f6e38c7) <br>

#### Word Cloud
We used it to Represent the most frequent genre of the anime in the dataset. Thus, as per the popularity we can get the most popular genre among people. <br>
![wordcloud](https://github.com/Manvn48/Anime-Data-Analysis/assets/142496783/62ca7bfe-fc8d-4349-bb1f-edcb8f2bc7db)

## TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) vectorization is a technique commonly used in natural language processing (NLP) to convert textual data into numerical vectors. It assigns weights to terms based on their frequency in a document and their rarity across all documents. 

- We utilized tf-idf vectorizer to convert the textual data (here anime genres) into numerical vectors.
- Each genre list is split into individual words or tokens.
- Here Using TF we measured how frequently a term (genre) occurs in a document (anime) while IDF measured the importance of a genre across the entire dataset.
- At last TF-IDF is obtained by multiplying the TF value by the IDF value for each term in the document.

## Cosine Similarity

Cosine similarity is computed between all pairs of anime based on their TF-IDF representations. <br>
So at last we measured the cosine of the angle between the two vectors that ranges from -1 to 1, with higher values indicating greater similarity.



  
