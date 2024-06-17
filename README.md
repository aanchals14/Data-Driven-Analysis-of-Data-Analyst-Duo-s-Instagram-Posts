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
     <img width="916" alt="Screenshot 2024-06-17 110054" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/45e153d6-66bb-496e-b74f-5f04837b2da2">
    - IG Reels outperform other post types with higher average reach (52605), impressions (43932), likes (1915), shares (680), saves (2178), and retention rate (67%), making them a valuable tool for engaging the audience and expanding reach on Instagram.
    - The average engagement rate for IG carousels is 9%, which is significantly higher than the engagement rate for IG images (5%) and IG reels (8%). This suggests that carousels are more effective at capturing users' attention and getting them to interact with the content.

2. Analysis 2: Engagement across Duration Bins
      <img width="914" alt="Screenshot 2024-06-17 110127" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/48f288f7-3197-46b1-9de0-2525c1042eb5">
    - Reels with a duration of less than or equal to 30 seconds are highly effective in terms of reach, impressions, comments, saves, and retention, indicating that shorter reels are more engaging and captivating for the audience.
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
1. Instagram Reach Over Time:

   <img width="386" alt="Screenshot 2024-06-17 140723" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/57616681-a2f8-4719-ab79-590c373cabd1">
  - The reach in 2022 and 2023 shows opposite trends, with 2022 peaking in March and August, while 2023 peaked in May.

2. Instagram Profile Visit Over Time:

   <img width="386" alt="Screenshot 2024-06-17 141046" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/2e2a23d5-1e66-43a2-ae49-0a3439096236">
  - In 2023, the peak in May indicates a strong interest or engagement spike, potentially due to specific content or campaigns during that period.
  - The declines in February to April and September to November in 2022 suggest periods of lower interest or engagement, possibly indicating the need for more engaging content or strategies during those months.

3. New Followers Gained Over Time:

   <img width="386" alt="Screenshot 2024-06-17 154959" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/810c117f-7f7b-4494-808e-46976cd88926">
   
  - The count of new followers is highest during December, May, July, and October irrespective of the year.

#### Demographic Analysis:
1. Age Distribution:

   <img width="386" alt="Screenshot 2024-06-17 150244" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/e4b395dc-cd52-4729-b6e5-3f0e5bb73709">
   
   - From the above bar graph, we can infer that the majority of followers are between 25-34. This age group is often highly active on social media platforms and may be more likely to engage with content.
   - They might also be a target demographic for the type of content or products/services this Instagram account promotes. 

2. Gender Distribution:

   <img width="386" alt="Screenshot 2024-06-17 145720" src="https://github.com/aanchals14/Instagram-Insights-Analysis/assets/131793044/218e9c61-af3c-4c34-a0eb-2e4bb25b87db">
   
   - The predominance of male followers could suggest that their content or brand resonates more with male audiences.
   - Understanding this demographic trend can help tailor their content strategy to better engage with their existing audience while also considering ways to attract a more diverse following if desired.

3. Geographic Distribution:

   ![FotoJet](https://github.com/aanchals14/Data-Driven-Analysis-of-Data-Analyst-Duo-s-Instagram-Posts/assets/131793044/6e732ab7-920a-4e5c-a48a-8d0ac5b9f6ff)
   - We could infer from the above most of the distribution is across South India and Maharashtra when it comes to the State-wise Distribution While in Country-Wise Distribution we see the majority of the audience are from India and the United States.
  
### Recommendations:
- Content Strategy Focus: Concentrate on creating more content related to Data Science, Data Analytics, SQL, Excel, Python libraries, Statistics, Online courses, Projects, Resume Building, Interviews, and Job Opportunities, as these topics resonate well with the audience.
- Engagement Optimization: Continue to prioritize IG Reels and IG Carousels in content strategy, as they tend to have higher reach and engagement rates.
- Audience Targeting: Tailor content to cater to the majority age group of 25-34, keeping in mind that the majority of followers are men.
- Geographic Focus: Since the majority of followers are from India, consider creating region-specific content or campaigns to further engage this audience segment.
- Consistent Analysis: Regularly analyze and compare data trends across months and years to adapt content strategy for optimal engagement and growth.

### Acknowledgement:
I would like to express my sincere gratitude to Data Analyst Duo for generously providing the dataset used in this analysis. Additionally, I am thankful to Kalpesh for his invaluable guidance throughout this project.
   

