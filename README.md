# Recommender-System-for-Movies
We have build a recommendation system for movies for the dataset containing information about movies and their ratings from 1995 to 2016. The user gives 5 movies with their ratings and the algorithm would give the recommendation of several similar movies taking into consideration the similar users and their choices of movies and ratings.

Recommendation systems are a collection of algorithms used to recommend items to users based on information taken from the user. These systems have become ubiquitous and can be commonly seen in online stores, movies databases and job finders. In this project, we will explore recommendation systems based on Collaborative Filtering and implement simple version of one using Python and the Pandas library.

**About the dataset**:

This dataset (ml-latest) describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 22884377 ratings and 586994 tag applications across 34208 movies. These data were created by 247753 users between January 09, 1995 and January 29, 2016. This dataset was generated on January 29, 2016.
Users were selected at random for inclusion. All selected users had rated at least 1 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.
The data are contained in four files, `links.csv`, `movies.csv`, `ratings.csv` and `tags.csv`.

Here is the first 5 elements of movies.csv and ratings.csv datsets

![Image of dataset1](https://camo.githubusercontent.com/6e1137b712b7b6feff75c56e72e483a74c8434f1/68747470733a2f2f686d702e6d652f64627635)

![Image of dataset2](https://camo.githubusercontent.com/8f97c05628a8d673db23d09cd2bddb475818e45e/68747470733a2f2f686d702e6d652f64627636)

We have done preprocessing before applying collabrative filtering to the raw data to get the recommendation results. The process we have followed for creating a User Based recommendation system is as follows:

- Select a user with the movies the user has watched
- Based on his rating to movies, find the top X neighbours
- Get the watched movie record of the user for each neighbour.
- Calculate a similarity score using some Pearson Correlation Algorithm 

![Image of equation](https://camo.githubusercontent.com/c522178708f3b90b4f505319031ce26309de2888/68747470733a2f2f686d702e6d652f64627637)

- Recommend the items with the highest score

We have generated top 10 recommended results for the following input:

**Input**

![Image of input](https://hmp.me/dbv8)

**Recommended Results**

![Image of output](https://hmp.me/dbv9)

