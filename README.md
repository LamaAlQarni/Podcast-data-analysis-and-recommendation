# Podcast Listening Behavior Analysis & Recommendation System
This project analyzes user listening behavior in a podcast platform dataset and builds a logic-based recommender system using user activity data, age group, and location.

## Data Loading & Processing
- No Missing Values.
- Discovered 13 records with a duration of 0 seconds (e.i. users accidentally opened a podcast episode without intending to listen).

## Data Analysis

**What are the most listened-to categories?**  
![Most listened-to categories](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/1-Most_listened-to_categories.png)

**How does listening duration differ by gender?**  
![Listening duration by gender](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/2-Listening_duration_by_gender.png)

**What’s the average number of episodes per user?**  
![Average number of episodes per user](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/3-Average_number_of_episodes_per_user.png)

**What are the most listened-to categories by gender?**  
![Most listened categories per gender](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/4-Most_listened_categories_per_gender.png)

**Which countries are the top listeners, and what do they prefer?**  
![Top listening countries](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/5-Top_listening_countries.png)  
![Top listening countries 2](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/5-2-Top_listening_countries.png)

**Which age group listens the most?**  
![Most listening age group](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/6-Most_listening_age_group.png)

**What is the most common episode duration users prefer?**  
![Most popular duration time for episodes](https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/7-Most_popular_duration_time_for_episodes.png)



## Recommendation Strategies
The goal is to recommend podcasts from the user’s favorite category, excluding episodes they've already heard. From the remaining pool, we apply three strategies to pick from the pool:
- **Random Recommendation**: Selects `k` random episodes from the same favorite category.
- **Demography-Based Recommendation**: select k episodes popular in the user’s country.
- **Age Group-Based Recommendation**: select k episodes popular among the user’s age group.



