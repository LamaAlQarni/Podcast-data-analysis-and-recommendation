# Podcast Listening Behavior Analysis & Recommendation System
This project analyzes user listening behavior in a podcast platform dataset and builds a logic-based recommender system using user activity data, age group, and location.

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
The goal is to recommend podcasts from the user’s favorite category, excluding episodes they've already heard. From the remaining pool, we apply three strategies to pick from the pool:
- **Random Recommendation**: Selects `k` random episodes from the same favorite category.
- **Demography-Based Recommendation**: select k episodes popular in the user’s country.
- **Age Group-Based Recommendation**: select k episodes popular among the user’s age group.



