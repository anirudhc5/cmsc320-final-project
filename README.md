# CMSC320 Final Project
Collaborators: Andrew, Anirudh, Ben, Kanishk, Sujan

## Our Topic

What determines high/low ratings of Movies/TV Shows on rating sites e.g. Rotten Tomatoes? More specifically, do Reddit conversations about a movie before its release predict its Rotten Tomatoes score after release?

## Our Datasets

1. Reddit posts and comments: Arctic shift archive (https://github.com/ArthurHeitmann/arctic_shift) API: https://arctic-shift.photon-reddit.com/api/posts/search from r/movies and r/boxoffice. A test data pull for the movie Dune returned 38 pre-release posts.
2. Movie ratings: OMDb API (https://www.omdbapi.com/) for Rotten Tomato Scores

## Our Data Plan

There's a free archive of all Reddit posts called Arctic Shift that goes back to 2023. We'd pull the posts and comments about hundreds of past movies from subreddits like r/movies and r/boxoffice, measure things like how much people talked about each movie and whether they sounded excited or skeptical before the movie actually released, and then check how well those measures line up with the scores the movies got post-release. We chose this dataset because this API essentially provides us the primary source for which we’re trying to accomplish our goal.

Additionally, we’ve chosen the OMDb API as a means of labeling/validating our data. Later on over the course of this project if we were to use semantic analysis to develop a predictive ML model on movie performance, this would be an excellent choice.

As an extra step, we could compare our predictions to Kalshi, where people can bet on what a movie's Rotten Tomatoes score will be. This idea is inspired by this paper (https://arxiv.org/pdf/1003.5699) from 2010, which says: “In particular, we use the chatter from Twitter.com to forecast box-office revenues for movies. We show that a simple model built from the rate at which tweets are created about particular topics can outperform market-based predictors. We further demonstrate how sentiments extracted from Twitter can be further utilized to improve the forecasting power of social media.”
