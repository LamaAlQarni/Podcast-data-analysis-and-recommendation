# Podcast Listening Behavior Analysis & Recommendation System
This project analyzes user listening behavior in a podcast platform dataset and builds a logic-based recommender system using user activity data, age group, and location.

## Data Loading & Processing
- No Missing Values.
- Discovered 13 records with a duration of 0 seconds (e.i. users accidentally opened a podcast episode without intending to listen).

## Data Analysis

**What are the most listened-to categories?**  
![Most listened-to categories](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/1-Most_listened-to_categories.png)

**How does listening duration differ by gender?**  
![Listening duration by gender](fig/2-Listening duration by gender.png)

**What’s the average number of episodes per user?**  
![Average number of episodes per user](fig/3-Average number of episodes per user.png)

**What are the most listened-to categories by gender?**  
![Most listened categories per gender](fig/4-Most listened categories per gender.png)

**Which countries are the top listeners, and what do they prefer?**  
![Top listening countries](fig/5-Top listening countries.png)  
![Top listening countries 2](fig/5-2-Top listening countries.png)

**Which age group listens the most?**  
![Most listening age group](fig/6-Most listening age group.png)

**What is the most common episode duration users prefer?**  
![Most popular duration time for episodes](fig/7-Most popular duration time for episodes.png)



## Recommendation Strategies
The goal is to recommend podcasts from the user’s favorite category, excluding episodes they've already heard. From the remaining pool, we apply three strategies to pick from the pool:
- **Random Recommendation**: Selects `k` random episodes from the same favorite category.
- **Demography-Based Recommendation**: select k episodes popular in the user’s country.
- **Age Group-Based Recommendation**: select k episodes popular among the user’s age group.



