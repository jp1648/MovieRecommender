# Movie Recommender
Collaborative Project with previous classmates.

Intro:

In our project, we are going to implement a recommendation system for movies. The way we envision this working is as follows: Suppose Person X enjoyed movie A. Based on
some parameters from movie A, we will ask our algorithm
to generate suggested movies. In return, we expect to get an
accurate list of movies similar to movie A. Similar to how
Netflix generates suggested movies based on past viewing
history and Spotify generates suggested music based on past
listening history, we aim to minimize the issue where a viewer
is stuck on what to watch next or where a viewer has no idea
where to start and wants to search for movies similar to a
specific title they have in mind. In our approach to building
our recommender system, we will utilize the MovieLens 20M
Dataset from GroupLens. This dataset has 20 million ratings
applied to 27,000 movies by over 135,000 users. The ratings
range from 1 to 5 and include the timestamp of the rating,
as well as other metadata like the movie genre and title. We
will implement this recommender system using three different
approaches. The first approach is known as “collaborative
filtering.” In collaborative filtering, we make predictions about
a user’s interests based on the preferences of other users. For
example, if user X likes movie A and movie B, and user
Y likes only movie A, we would recommend movie B to
user Y since user X also liked movie A and enjoyed movie
B. Essentially, with collaborative filtering, we assume that
since users have agreed in the past, they will also agree in
the future. Collaborative filtering can be of two types: user-
based or item-based. In user-based collaborative filtering, we
make recommendations based on similarities between users.
To compute the similarity between users, we will find the
cosine similarity. After computing the similarity measure, we
will find users similar to each other and recommend items that
similar users have liked in the past, which the target user has
not interacted with. In item-based collaborative filtering, we
find the similarity between movies themselves. The steps are
similar to user-based collaborative filtering: first, we compute
the similarity between movies using cosine similarity based
on features of the movies. Then, we find similar movies and
ultimately suggest movies similar to the ones that the target
user has previously liked. The second approach is known as
“content filtering.” Content filtering is similar in some ways to
collaborative filtering, but it uses a representation of a user’s
preferences as dictated by their past behavior, from likes to
searches, to recommend content. In our case, we will use data
like a user’s searches, liked movies, and recently watched
movies. For example, if a user searched for movie A and
watched movie B, and another user watched both movies
and liked movie C, we would recommend movie C to the
searcher. Finally, our third approach will utilize a hybrid of
both collaborative and content filtering. As mentioned before,
while collaborative filtering could be user-based or item-based,
and content filtering is based on a user’s past behavior, our
third approach will combine these algorithms to recommend
movies. There are many ways in which this could work,
including the weighted hybrid model, mixed hybrid model, and
cascade hybrid model. In a weighted hybrid model, we assign
weights to each model to see which combination works best
in recommending movies. In a mixed hybrid model, we use
features of both collaborative and content filtering to form the
recommendation system, and in a cascade hybrid model, we
use one method to refine the recommendations of the other. Al-
together, our approach is focused on utilizing a filtering mecha-
nism to find similarities between various users and recommend
films to a user. By using different filtering algorithms, we aim
to create a robust system to recommend movies similar to the
ones in a user’s search criteria. This system will continue to
learn and feed information to help recommend movies to other
users. Through our use of collaborative filtering, we have been
able to witness our algorithm accurately suggest movies of
similar genres based on users’ search criteria. We specifically
focused on using only users’ ratings to generate search results
for other users. Throughout various popular applications like
Netflix, Spotify, and even Facebook, recommendation systems
have been prevalent. Movie recommendation systems enhance
user experience using methodologies like collaborative filtering
(user-based and item-based) and content-based filtering. Re-
cent advancements include hybrid models combining these ap-
proaches, matrix factorization techniques like SVD, and deep
learning methods such as neural collaborative filtering and
autoencoders. Our project aims to build on these methods using
the MovieLens dataset to create a tailored recommendation
system. Ultimately, we believe this recommender system can
perform better than existing solutions because of our use of
different hybrid approaches, which will combine the strengths
of different filtering types.
