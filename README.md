# Recommender System

# Project Overview
This project was done as part of my Data Science Practicum II to better understand the process of designing a recommendation system.

Recommendation Systems are used in various industries to provide recommendations for products such as movies and books.
These recommendations are based on finding similaties in items and/or users to recommend a product that might be of interest to the 
user.  

# Data Observations

* The data was obtained from http://www2.informatik.uni-freiburg.de/~cziegler/BX/
* The data contained three files:
  1) BX-Books - 271,380 observations
  2) BX-Users - 278,858 observations
  3) BX-Book-Ratings - 1,149,780 observations
 
# Data Cleaning Approach

 * Inital matrix size was 75,670,906,880 and sparsity of the matrix was very high at 99.9%.
   In an effort to reduce the matrix size I performed the following:
   1) Removed the ratings with no associated book
   2) Removed books with overall total rating less than 50
   3) Included books from USA only


# Data Composition

After the data cleaning was complete, the data consisted of the following:

* Distribution of Age of users:

![Age Distribution](https://github.com/dvroman22/RecSys/blob/master/distage.png)

* Distribution of Book Ratings of users:

![Book Rating Distribution](https://github.com/dvroman22/RecSys/blob/master/distrtplot.svg?sanitize=true)

 * Distribution of Ratings counts: 
 
![Summary of Ratings](https://github.com/dvroman22/RecSys/blob/master/numrtplot.svg?sanitize=true)

# Recommendation System Approaches - Collaborative Filtering

* Produce simple popularity based recommendation system
* Produce KNN with cosine similarity recommendation system using scikit-nearest neighbors
* Produce Singular Value Decomposition (Dimensionality Reduction) recommendation system using scikit Truncated SVD
* Utilize the Surprise Library to analyze and build recommendations

# Modeling Analysis

* Benchmark available algorithms in the Surprise libary to determine lowest RMSE
* Display specific books to determine if the recommendations made sense


![Alt text](https://github.com/dvroman22/RecSys/blob/master/algoplt.svg?sanitize=true)


# Conclusions

* Data preparation for the recommender algorithms was very important and took some research and understanding
* Many algorithms exist in ML tools and benchmarking the different algorithms proved to be very helpful in my analysis
* The recommendation from the various recommender approaches I used seemed to work fairly well and made sense, for the most part
* The Surprise Library had many algorithms to choose from and the documentation was extemely helpful

# YouTube Link

https://youtu.be/XXuGWZgkUE0

