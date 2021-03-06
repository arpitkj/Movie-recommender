# Movie Recommendation System
&nbsp;
![movie collage](https://miro.medium.com/max/1797/1*FY2Rb_upY-_m61tFsh8T1w.png)
&nbsp;

## Overview
Recommender System is a system that seeks to predict or filter preferences according to the user’s choices. Recommender systems are utilized in a variety of areas including movies, music, news, books, research articles, search queries, social tags, and products in general. 
Recommender systems produce a list of recommendations in any of the two ways – 
 
* __Collaborative filtering:__ Collaborative filtering approaches build a model from the user’s past behavior (i.e. items purchased or searched by the user) as well as similar   decisions made by other users. This model is then used to predict items (or ratings for items) that users may have an interest in.
* __Content-based filtering:__ Content-based filtering approaches uses a series of discrete characteristics of an item in order to recommend additional items with similar properties. Content-based filtering methods are totally based on a description of the item and a profile of the user’s preferences. It recommends items based on the user’s past preferences.

I have implemented a movie recommender system that follows the underlying principles of collaborative filtering (similar to what Netflix or Amazon uses), applying __Singular Value Decomposition (SVD)__, __Cosine Similarity__, and __Principal Component Analysis(PCA)__.

## Dataset

The details of the movies (title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB: https://www.themoviedb.org/documentation/api

Sources of the dataset include:
1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

## Technical Aspect

* Firstly, i made a matrix with all the movies against all the users.
* Next, I normalised it and computed SVD.
* Then, cosine similarity as claculated and top results are shown as recommendations.
* Lastly, the model was deployed on Heroku using Flask.
&nbsp;
<img src="https://miro.medium.com/max/1313/1*x8gTiprhLs7zflmEn1UjAQ.png" width="700" height="700">
&nbsp;

## Tech Stack

* Pandas
* NumPy
* Jupyter
* Flask

