# Movie_recommender_documentation
I have build a movie recommender engine using python

There can be two types of recommendation system

       1)content based filtering(which I have implemnted in this project)
       
       2)collaberative filtering(more efficient)
       
   In content based filtering the suggestions are based on what all types of movies the user watches and which movies are most similar to what the user generally watches.Content-based approaches attempt to build a user profile to predict ratings on unseen items.Successful content-based methods utilize tags and keywords. In the I measured the utility of content-based filtering  by using heuristic functions, i.e the cosine similarity metric.

       
  In my project I have implemented *content based filtering* using co-sine function similarity.
  
   After preprocessing the data which I downloaded from kaggle, the movies had  particular tags or u can say category words then I performed vectorisation and then in order to recommend the I just had to find the most closest vectors to the given film. Here we can calculate the distances of all vectors from the given movie vector and simply sort the data brought from this search and recommend the first 5 or 10 movies as per the interface requirements.
   
   # Why only cosine similarity?
   
   As the movie dataset contains a large number of movies, so we would be left with a large number of movie vectors in 3d space and calculating euclidean distance becomes insignificant and irrelavant due time and space factors. So cosine distance i.e cosine of the angle is taken as a measure of distance.



  # Role of Search algorithms

While writing a code for recommendation, the use effective search algorithm is very crucial as we need to be fast to scan the various datasets as early as possible and find the similar datasets and recommend it to user faster



  # Role of Sorting algorithms

Sorting or matching algorithms play a very crucial role in any recommendation engine.

    for example I search for the word orange colour in my recommendation engine, let say google. So, the search algorithms would effectively search for all the links, datas containing orange or containing color or both. So, the sorting algorithms are the one which will reorder and hence find the best matches to the searched word and would recommend it first.

use of effective sorting algos is hence important for faster and smoother experience of the user.
As a beginner, I feel *quick sort* is an effective algorithm as for its average time complexity and more efficiency when we have a quite large data.

# Any other approach

I have built a simple recommendation engine just using jupyternotebook and streamlit library. Due to time constraints I wasnt able to give more research to the project.

But i would further use some of my approaches like arranging all the data set into graphs and using the algorithm of finding nearest neighbour.
Also implementing various search algorithms and see thier accuracy and time of execution on different range of data sets.

# What about collaberative filtering?

This method combined with content filtering is actually most used by various streaming platforms nowadays.
In this type of recommendation system, all the close connected users are searched and movie is recommended based on what the other similar users like.
This more efficient way of reccomendation as it combines interest of people very similar to you to reccomend the movie.
