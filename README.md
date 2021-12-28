# Netflix-Recommender-System

***Problem Definition***
Recommendation systems can be thought of as a subclass of information filtering systems that attempt to forecast a user preference for a particular item (Elena.cuoco, 2017), in this case, a movie. Our recommender system has two parts — first, to complete the matrix with predicted user ratings. Next, to recommend a list of movies based on the user’s previous interactions with the system. 
While this particular project focuses on recommender systems for Netflix movies, this project can be deployed in a variety of areas. 

Numerical Technique used
We will be using Alternative Least Squares for recommender systems based on matrix factorization. There are two steps towards finding the predictions of R. First, we employ matrix factorization and split the ratings matrix R into two smaller matrices — X, the user matrix and Y, the item matrix. In order to predict the user’s rating for each individual item i, we do the following: Ui ≈ XiT · Yi . We are able to find the predicted matrix of user ratings U through minimizing the error function, as shown in Figure 0.4, and finding the suitable X and Y which through the equation Ui ≈ XiT · Yi is as close as possible to the matrix R with accurate user ratings in place of NaN values.

Results
We saw that the recommendation system was able to accurately predict the user ratings in place for the unknown values (NaN values) in the ratings matrix with minimal error. In addition to this, it was able to recommend several movies based on the user's feedback to previous movies.
