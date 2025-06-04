# Podcast Listening Behavior Analysis & Recommendation System
This project analyzes user listening behavior in a podcast platform dataset and builds a logic-based recommender system using user activity data, age group, and location.


## Summary and Results
+ **Popularity Peaks**: The categories "Society" and "Sport" dominate the platform, attracting over 65% of total listeners.
+ **Gender Listening Patterns**:<br>
   A noticeable difference emerges between genders:<br>
      - **Women** prefer longer content, averaging **15.1 minutes**.<br>
      - **Men** prefer shorter content, around **10.4 minutes**.<br>
+ **Engagement Levels**: On average, a user listens to **4.5 episodes** (decent level of retention, but can be improved).
+ **Top Geographies**: Nearly **half of the audience** comes from **Jordan and Morocco**. These countries should be prioritized for targeted content
+ **Preferred Episode Durations**: Listeners highly favor **shorter episodes**, especially **1-minute and 5-minute** episodes.
+ **Age Demographics**: A significant **71% of listeners are above 30 years old** (you have a mature audience base :0).
+ **Underperforming Categories**:  **"Technology"** and especially **"Politics"** are the **least engaging categories** across all regions. 

<hr>


## Data Loading & Processing
- No Missing Values.
- Discovered 13 records with a duration of 0 seconds (e.i. users accidentally opened a podcast episode without intending to listen).

## Data Analysis
This analysis answers the 7 questions below:

**1. What are the most listened-to categories?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/1-Most_listened-to_categories.png?raw=true" width="450">

**2. How does listening duration differ by gender?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/2-Listening_duration_by_gender.png?raw=true" width="450">

**3. What’s the average number of episodes per user?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/3-Average_number_of_episodes_per_user.png?raw=true" width="450">

**4. What are the most listened-to categories by gender?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/4-Most_listened_categories_per_gender.png?raw=true" width="800">

**5. Which countries are the top listeners, and what do they prefer?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/5-Top_listening_countries.png?raw=true" width="450">  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/5-2-Top_listening_countries.png?raw=true" width="800">

**6. Which age group listens the most?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/6-Most_listening_age_group.png?raw=true" width="600">

**7. What is the most common episode duration users prefer?**  
<img src="https://github.com/LamaAlQarni/Podcast-data-analysis-and-recommendation/blob/main/fig/7-Most_popular_duration_time_for_episodes.png?raw=true" width="600">


## Personalized Recommendation Strategies
The goal is to recommend podcasts from the user’s favorite category, excluding episodes they've already heard. From the remaining pool, we apply three strategies to pick from the pool:
- **Random Recommendation**: Selects `k` random episodes from the same favorite category.
- **Demography-Based Recommendation**: select `k` episodes popular in the user’s country.
- **Age Group-Based Recommendation**: select `k` episodes popular among the user’s age group.


    



