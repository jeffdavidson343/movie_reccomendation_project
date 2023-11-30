# movie_recomendation_project
UCF Bootcamp Final Project

Authored by Jeffrey Davidson, Steven Marsicek, Juan Suarez, and Richard Slader Torres

Introduction
---
For our project we decided to use machine learning to make better movie recommendations. 
Based on the MovieLens 1M dataset from GroupLens Research, our team has created a model that provides better reccomendations than the most seasoned movie buffs.

1. We started by using tableu to explore the data, see if we could find any trends that would influence our recommendations.
What we found is that movie ratings are extremely biased, and only represent a small portion of the population.
By using machine learning we can offer better recommendations that are based on a users ratings history, instead of their demographics.

2. Next we moved on to cleaning the data. This involved reading in all the csv's to dataframes, merging dataframes,
and modifying columns to optimize for encoding & machine learning.

3. Next we started building our first model. We decided to start off using the Nearest Neighbors model,
because it calculates a score and a “distance” that we can then use to make suggestions. We fed in our data Set of Users and their reviews of all movies into a nearest neighbors model.
The function then takes input from user of a movie name. Based on that user input a list of the top 10 shortest distances generated and stored in the model are produced.

4. Finally, we optimized our model to provide the best possible recommendations. Firstly, we utilized elbow curve testing to determine the optimal K value for our model.
We also noticed our original data set was giving equal weight to every review, causing some movies to be recommneded too often. To solve this, we filtered our data to
only include movies with >7 reviews. We also only considered ratings from users that have left more than 40 reviews.
This filtering still left us with 3,319 unique reviewers, and 4,690 movies for our model.

Instructions
---
Instructions for Nearest Neighbors Model
1. Download CSV's Stored in the main folder along with "recomendation" jupyter notebook.
2. Open recomendation notebook and run all lines of code up to codebox 12 
3. In code box 12, enter a movie title in the quotes in the "Get Movie recomendation" fucntion
4. Enjoy the results
