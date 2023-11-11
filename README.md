# PROJECT-SOCIAL-BUZZ

# BUSINESS QUESTION

This project revolves around the examination of 'Social Buzz,' a company that is progressively evolving into a global unicorn enterprise. Their platform routinely receives an influx of over 100,000 posts daily, aggregating to a staggering 36,500,000 posts annually. Notably, this data is predominantly unstructured, rendering it complex to extract meaningful insights. The key focus of this analysis is to highlight the top 5 content categories within this datasets.

# DATASETS

There are 3 datasets provided for this analysis.
Content Dataset – The Content dataset consists of the following column names: Content ID, User ID, Type, Category, and URL.
   
Reactions Dataset - The Reactions dataset consists of the following column names: Content ID, User ID, Type, and Datetime

Reaction Types Dataset- The Reaction Types dataset consists of the following column names: Type, Sentiment, and Score.
   
# DATA CLEANING AND TRANSFORMATION

* I refined our datasets by removing unnecessary columns and rows that didn't pertain to the primary business question. This included the removal of the ‘URL’ and ‘User ID’ columns in the Content dataset, as well as the ‘User ID’ column in the Reactions dataset. Blank rows, which were not relevant to our analysis, were also removed from all three datasets.
*	I standardized the column names across the datasets to ensure consistency. Specifically, I replaced the 'Type' column in the Content dataset with 'Content Type' and made the same adjustment in the Reactions and Reaction Types dataset, where 'Type' became 'Reaction Type'. 
*	In addition, I removed quotation marks from ‘categories’ column in the Content dataset to maintain a uniform naming convention.
   
**Note:** Data cleaning was done using Ms Excel.

# DATA ANALYSIS

* I created a finalized dataset titled 'Clean Merged Dataset' by merging information from the Content, Reactions, and Reaction Types datasets. This merging process was executed using the ‘VLOOKUP’ formular within Ms Excel, with the Reaction Table serving as the base table.
   
![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/d5023c88-2cb8-4540-bdc8-b4ef409e4629)

* In order to identify the top 5 categories, I computed the cumulative scores for each category by applying the 'SUMIF' formula in Microsoft Excel.
   
![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/0959c145-35cc-4284-9f70-327d068c04a6)

* See below Top 5 categories
  
![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/6e167626-5c89-4b1b-9a2a-84aab325d22f)

# DATA VISUALIZATION
A user-friendly and interactive dashboard has been developed using Power BI to present the results of this data analysis. 

![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/7e68e580-7ac0-4bac-adbf-946d833c3e0f)

# INSIGHTS AND CONCLUSION
* Upon analyzing the data, I have identified 16 distinct content categories. My findings confirm that the five most popular categories of posts are, in order of popularity: Animals, Science, Healthy eating, Technology, and Food.

* 'Animals' stands out as the leading category, amassing a total reaction score of 1,897. Within this category, there are 570 audio posts, 342 GIFs, 674 photos, and 311 videos. This indicates a strong affinity among our audience for animal-related content.

* The presence of both 'Food' and 'Healthy Eating' in the top 5 is intriguing, emphasizing the strong engagement with food-related content. Healthy eating, ranking just above food, suggests that our user base might lean towards health-conscious individuals.

* The inclusion of 'Science' and 'Technology' in the top 5 highlights a preference for informative content that offers learning opportunities.

* Our data reveals that January is the most common month for users to post content. This aligns with the seasonal trends of social media users, as they tend to reconnect with others after major calendar events like Christmas.

# RECOMMENDATIONS
* The prevalence of "Food" among the top 5 categories provides valuable insights into our user base. This knowledge can be strategically used to enhance engagement. Collaborating with Healthy Eating brands, influencers, restaurants, and relevant social media entities presents an opportunity to amplify favoured content, subsequently increasing user reactions.

* 'Animals' and 'Science' stand out as the top two categories, signifying a strong user preference for 'real-life' and 'factual' content. I recommend that the business should consider launching educational campaigns or series within the 'Science' category to provide users with valuable and informative content. This aligns with user interests and is likely to garner higher engagement.

* The analysis of the sentiment paints a clear picture: a significant 84.64% of users express positive satisfaction, 8.71% remain neutral, and 6.65% express negative sentiments. Based on this data, I would make the following recommendations;
* Capitalize on the huge positive sentiment by highlighting and promoting content that resonates with users. This can include positive user reviews, success stories, or uplifting content.
* Pay attention to the 6.65% with negative sentiment. Investigate the reasons behind it, whether it's related to specific content, user experiences, or other factors. Take steps to address these issues to improve user satisfaction.
* Explore the content that falls under the neutral sentiment category. Consider ways to make it more engaging or informative to potentially shift it towards a positive sentiment.

Dataset from theforage.com (Accessed: July 2023)
