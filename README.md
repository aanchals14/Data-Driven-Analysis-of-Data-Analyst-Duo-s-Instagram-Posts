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
#### Content Analysis:
1. Analysis 1: Engagement across Different Post Types
     <img width="916" alt="Screenshot 2024-02-22 193834" src="https://github.com/aanchals14/Data-Driven-Analysis-of-Data-Analyst-Duo-s-Instagram-Posts/assets/131793044/f82b1dad-aa65-474b-bc66-63f944361379">
    - IG Reels outperform other post types with higher average reach (52605), impressions (58707), likes (1915), shares (680), saves (2178), and retention rate (56%), making them a valuable tool for engaging the audience and expanding reach on Instagram.
    - The average engagement rate for IG carousels is 9%, which is significantly higher than the engagement rate for IG images (5%) and IG reels (8%). This suggests that carousels are more effective at capturing users' attention and getting them to interact with the content.

2. Analysis 2: Engagement across Duration Bins
      <img width="914" alt="Screenshot 2024-02-22 195503" src="https://github.com/aanchals14/Data-Driven-Analysis-of-Data-Analyst-Duo-s-Instagram-Posts/assets/131793044/d471399f-3aa9-42d8-b8ac-db6a8e445550">
    - Reels with a duration of less than or equal to 30 seconds are highly effective in terms of reach, impression, comments, saves, and retention, indicating that shorter reels are more engaging and captivating for the audience.
    - Reels with a duration of more than 30 seconds are particularly effective in generating likes, shares, and overall engagement, suggesting that longer reels may allow for more detailed or immersive content that resonates well with the audience.

3. Analysis 3: Analysed important keywords for highest-performing posts
   - The posts were categorized based on the impression bins created: Below 10k, 10k-50k, 50k-1lakh, and Above 1 lakh.
   - Word clouds were created for each of the bins to visualize the frequency of the keywords and the frequently occurring keywords were identified from them.
     ![keyword](https://github.com/aanchals14/Data-Driven-Analysis-of-Data-Analyst-Duo-s-Instagram-Posts/assets/131793044/6e8e9967-d9b6-4195-95d7-a32523eca856)
   - It was found that the majority of the posts fell in the Below 10k and 10k-50k bins which suggests that a significant number of posts are not reaching a large audience, as they fall within the lower impression bins.
   - Posts may be receiving a significant number of impressions (falling in the below 10k and 10k - 50k impression bins), they may not be effectively optimized with keywords to maximize engagement and reach.

4. Analysis 4: Analyze important keywords for posts with high follows
   - The Posts were categorized on the basis of the follow bins created which are : 0-50, 50-200, 200-500, 500-1000 and 1000+. Word clouds were generated to see the frequency of keywords in the posts with highest number of follows.
     ![keyword_2](https://github.com/aanchals14/Data-Driven-Analysis-of-Data-Analyst-Duo-s-Instagram-Posts/assets/131793044/528c8a58-8fb4-4fcb-8281-3df05b2ef0e2)
   - Majority of the posts fall in the 0-50 follows bin, indicating a potential need to diversify the content strategy to attract a broader audience.
   - The keywords do not show a clear pattern across different follow bins, suggesting that factors other than keyword usage may influence post performance.
   - Experiment with various content types to determine the most effective ones for different follow bins. Monitor engagement metrics, particularly for posts with 0-50 followers, to detect trends and adjust the content strategy accordingly.

#### Daily Statistics Analysis: 
1. Instagram Reach Over Time
   



