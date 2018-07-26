# Recommender System

This project showcases how to do a recommendation system. The main goal is to provide users with 
information about movies they might find interesting. The project explores a collaborative filtering 
approach that yields viable recommendation results.

## Introduction

Companies are creating a well crafted, perfectly curated online experience that caters to the taste 
and needs of each individual user. Every company that offers a product is bound to recommend more 
items that might be of interest to the user. For example, Amazon recommends that extra book that the 
user did not search for but ended up buying. Netflix recommends a show related to the one that the 
user just binge watched to keep the user engaged. All this is possible thanks to recommendation 
systems.

Recommender systems personalize a user's experience on a platform, telling what to buy, where to 
eat, what to watch, or who to be friends with. These systems capture patterns in the data that help 
predict suggestions that keeps the user engaged. From online news to e-commerce websites, everybody 
is making sure their customers are efficiently served with the right products. 

The goal of a recommendation model is to present a ranked list of objects given an input object. 
There are different methods to approach this problem. Two of the most commonly used approaches are 
Content-Based and Collaborative Filtering. For this project, we will focus on Collaborative filtering method which is based on the relationship between users and the items. 

## Dataset

The data used for this project was the MovieLens 100K Dataset which contains 
100004 ratings and 1296 tag applications across 9125 movies. The data was acquired 
from the following source:

- [MovieLens](http://grouplens.org/datasets/movielens/)

## Recommendation System

### Technique

There are many ways of building a recommender system. This project went over two different ways of implementing Collaborative Filtering. We covered Memory-based models which are based on similarity between items or users, where we used centered cosine-similarity, also known as pearson correlation.

### Results

| CF Algorithms | RMSE          |
|:-------------:|:-------------:| 
| Use-Based     | 3.586         | 
| Item-Based    | 3.542         |  

Item-based collaborative filtering performed better than user-based. In practice, item-based tends to outperform user-based for most use cases, such as movies. This is because items are simpler than users since they belong to a small set of genres like seen in the data analysis step.
