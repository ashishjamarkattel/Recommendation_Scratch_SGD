
# Recommendation System - SVD,Matrix Factorization
#### This repo is for implementation of matrix Factorization from scratch using Singular Value decompostion with optimizer SGD.
###
Recommendation system is type of system that has ability to recommend. 
Recommendation can be of various things like you recommending your friend 
to buy something that you like or u recommending your friend to watch the series you watch. 

This kind of recommendation helps to make user experience easy and less time consuming as you dont have to spend much time surfing internet that you like. This is the reason why big internet company pays a big chunk of money in building the best recommendation system in their product.

There are generally two type of recommendation system.

- Content based.
- Collaborative filtering.

Since Content based is easy as it can be translated in the regression or classification problem.
Regression  when we have to predict the rating of the movie by the user and Classification when we have to predict what might user like .

Note: It is mostly domain specific whether or not you want to formulate your problem as Regression or Classification.


In this we typically have information 
about the user. The information might be 

    1. Geo location.
    2. Device he is using.
    3. Surfying from.
    4. Have taste in which product and many more.


As this post is not about regression or classification we will mostly focus on Collaborative filtering type of 
recommendation system.
Recommending using collaborative include Cosine similarity computation or  Knn distance Calculation.
But in this article is will be discussion about  Matrix Factorization.

### Matrix Factorization

Matrix Factorization is decompostion of higher matrix in smaller matrix. I usually seems this problem as (a+b)^2 = (a^2+2ab+b^2) as here also bigger function are broken down in to smaller subset to get eact values which reduce computaion and is less time comsuming.
So, by that we have clear understanding if we break the higher matrix we can compute faster.So this is the basic idea of decomposition i.e Factorization.

### So How does this thing is useful in recommendation sytem?
Ans is simple as we have the sparse matrix of the A with B. we could fill the sparsness of the matrix just by predicting whether or not user would like the item B which he has never tasted.
###
let take the example of netflix.

User will not have seen all the movie present in the netfilx so matrix will be sparse. So how do we identify if user will like the movie or not.
Here where Matrix Factorization comes in handy.

In this case matrix Factorization comes handy.



## Optimizations

Since __SGD__ - Stochastic gradient descent is slow, so to implement this I also tried something like 
Alternative Stochastic gradient descent which is an Alternative approch to SGD where at a time only one variable is updated.
As this is only for implement and learning i only optimize some of the bais in the loss.You can try to optimze other variable too.
