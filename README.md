# Podcast Listening Behavior Analysis & Recommendation System
This project analyzes user listening behavior in a podcast platform dataset and builds a logic-based recommender system using user activity data, gender, age group, and location.

## Data Loading & Processing
- No Missing Values.
- Discovered 13 records with a duration of 0 seconds (e.i. users accidentally opened a podcast episode without intending to listen).

## Data Analysis
1. What are the most listened-to categories?
2. How does listening duration differ by gender?
3. What’s the average number of episodes per user?
4. What are the most listened-to categories by gender?
5. Which countries are the top listeners, and what do they prefer?
6. Which age group listens the most?
7. What is the most common episode duration users prefer?

## Recommendation Strategies
As the assignment prompt encouraged us to recommend podcasts to users based on their favorite content category. 
We made a recommnedation list of episodes with the same favorite content category but filtered out those already listened to by the user.
This left us with a bunch of episodes to pick from, the following are the strategies used to pick from the list:
- **Random Recommendation**: Selects `k` random episodes from the favorite category.
- **Demography-Based Recommendation**: select k episodes that people from the *same country* most listened-to.
- **Age Group-Based Recommendation**: select k episodes that people from the *same age group* most listened-to.



