# Instagram Insights Analysis
Data-Driven Analysis of Data Analyst Duo's Instagram Posts

### Introduction:
This report presents the design and implementation of a data-driven Instagram engagement analysis dashboard for Data Analyst Duo's Instagram account (@dataanalystduo). The dashboard aims to provide insights into the performance of different post types to enhance engagement strategies.

### Objectives:
The project focuses on two primary objectives:
  1. To design and develop a dashboard that visualizes key Instagram engagement metrics for Data Analyst Duo's account, which has approximately 104,000 followers.
  2. To analyze the performance of different post types and guide content strategy for improved engagement.

### Data Cleaning & Preparation:
1. The dataset included three sheets containing data on reach, Instagram follower visits, and new followers from 9 January 2022 to 27 October 2023, all of which were prepared for analysis.
2. A consolidated datasheet named "Daily Stats" was created by merging the reach, Instagram follower visit, and new followers datasets using VLOOKUP from 9 January 2022.
3. The total follower count was determined by subtracting the number of new followers from the count on 27 October 2023. Subsequently, the remaining rows were calculated using a cumulative sum approach.
4. Growth Rate: The percentage change in the number of followers on an Instagram account over a specific period. 
  - Growth Rate = ((Current Follower Count - Previous Follower Count) / Previous Follower Count) * 100
5. The Content stat dataset included content and engagement metrics data, such as likes, shares, comments, saves, reach, and impressions, spanning from 1st December 2022 to 27 October 2023.
6. New key performance indicators (KPIs) were introduced to the Content stat dataset, including Engagement Rate, Retention Rate, and Interaction Rate, to enhance the analysis of content and engagement metrics spanning from 1st December 2022 to 27 October 2023.
    - Engagement Rate: The percentage of followers who interact with your Instagram content (likes, comments, shares, saves) relative to the total number of followers.
      - Engagement Rate = (Like +Comment +Share +Save) / Reach *100
    - Retention Rate (Reel): The retention rate for Instagram Reels measures the percentage of viewers who watch a reel for more than 3 seconds, indicating viewer engagement and interest.
      - Retention Rate = (3s views / impressions) * 100
    - Interaction Rate: The interaction rate on Instagram measures the percentage of followers who engage with a post through likes, comments, and shares, relative to the total reach of the post.
      - Interaction Rate = (Total likes + comments + shares) / Total reach * 100
7. Duration bins were created to evaluate the performance of reels, with two categories established: less than 30 seconds and 30 seconds or more.
    - Below 10k
    - 10k - 50k
    - 50k - 1 Lakh
    - Above 1 Lakh
8. Impression bins were calculated to analyze important keywords for high-performing posts.
    - 0 - 50
    - 50 - 200
    - 200 - 500
    - 500 - 1000
    - 1000 +

### Analysis & Insights:





