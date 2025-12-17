# CODTECH-Task4

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: SK ALTAB HOSSEN

*INTERN ID*:CT04DR1863

*DOMAIN*:MACHINE LEARNING

*DURATION*: 4 WEEKS

*MENTOR*:NEELA SANTOSH

##Task 4: Recommendation System
Project Description

Title: Movie Recommendation System using Item-Based Collaborative Filtering**

Introduction Recommendation systems are algorithms designed to suggest relevant items to users. They are ubiquitous in the digital world, powering platforms like Netflix, Amazon, and Spotify. Broadly, these systems are categorized into Content-Based Filtering (recommending items similar to what a user liked before) and Collaborative Filtering (recommending items based on the preferences of similar users). For this task, I implemented an Item-Based Collaborative Filtering system.

Methodology The core idea behind Item-Based Collaborative Filtering is "Users who liked this item also liked that item." It does not rely on item metadata (genre, director, etc.) but purely on user interaction patterns (ratings).

Data Structure: I created a synthetic dataset representing a User-Item Matrix. In this matrix, rows represent users, columns represent movies, and the values represent the ratings (1-5 stars) a user gave to a movie.

Similarity Metric (Cosine Similarity): To find similar movies, I calculated the Cosine Similarity between the rating vectors of every pair of movies. Geometrically, if two movies have similar ratings from the same set of users, their vectors will point in the same direction, resulting in a cosine similarity score close to 1. If their ratings are unrelated, the score is close to 0.

Recommendation Logic: The system takes a specific movie (e.g., "Inception") as input. It looks up the similarity scores for all other movies relative to "Inception" and sorts them in descending order. The top-ranking movies are then returned as recommendations.

Results The system successfully identified relationships between items. for example, in the synthetic data, users who rated "Inception" highly also tended to rate "Matrix" highly. Consequently, when the system was queried with "Inception," it recommended "Matrix." This demonstrates how collaborative filtering can uncover hidden patterns in user behavior to provide personalized experiences without needing to understand the content of the items themselves.

#OUTPUT
