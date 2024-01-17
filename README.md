# Business Question

This project revolves around the examination of 'Social Buzz,' a company that is progressively evolving into a global unicorn enterprise. Their platform routinely receives an influx of over 100,000 posts daily, aggregating to a staggering 36,500,000 posts annually. Notably, this data is predominantly unstructured, rendering it complex to extract meaningful insights. The key focus of this analysis is to highlight the top 5 content categories within this datasets.

# Datasets

There are 3 datasets provided for this analysis.

Content Dataset – The Content dataset consists of the following column names: Content ID, User ID, Type, Category, and URL.
   
Reactions Dataset - The Reactions dataset consists of the following column names: Content ID, User ID, Type, and Datetime.

Reaction Types Dataset- The Reaction Types dataset consists of the following column names: Type, Sentiment, and Score.
   
# Data cleaning and transformation

* I refined the datasets by removing unnecessary columns and rows that didn't pertain to the primary business question. This included the removal of the ‘URL’ and ‘User ID’ columns in the Content dataset, as well as the ‘User ID’ column in the Reactions dataset.
* Blank rows, which were not relevant to the analysis, were also removed from all three datasets.
*	I standardized the column names across the datasets to ensure consistency. Specifically, I replaced the 'Type' column in the Content dataset with 'Content Type' and made the same adjustment in the Reactions and Reaction Types dataset, where 'Type' became 'Reaction Type'. 
*	In addition, I removed quotation marks from ‘categories’ column in the Content dataset to maintain a uniform naming convention.
   
**Note:** Data cleaning was done using Ms Excel.

# Data analysis

I created a final dataset titled 'Clean Merged Dataset' by merging information from the Content, Reactions, and Reaction Types datasets. This merging process was executed using the ‘VLOOKUP’ formular within Microsoft Excel, with the Reaction Table serving as the base table.
  
![image](https://github.com/OluwatobiAkintokun/PROJECT-SOCIAL-BUZZ/assets/137109080/68208dad-3e1c-49c6-b878-91720ed71187)
  
In order to identify the top 5 categories, I computed the cumulative scores for each category by applying the 'SUMIF' formula in Microsoft Excel.
   
![image](https://github.com/OluwatobiAkintokun/PROJECT-SOCIAL-BUZZ/assets/137109080/d50b27fb-3ef5-48b3-88a4-e7502904ec47)

# Data Visualisation


**Top 5 Categories**

Below is a column chart and pie chart, showing the top 5 categories in actual numbers and percentages.

![image](https://github.com/OluwatobiAkintokun/PROJECT-SOCIAL-BUZZ/assets/137109080/84d9c2a3-ce6c-45b9-ba69-67557337d504)


**Dashboard**

A user-friendly and interactive dashboard has been developed using Power BI to present the results of this data analysis. [View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOGE4N2YyMWMtNjFhOC00MTUyLThlZDMtZGFmNWNhZWZmZjIxIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

![image](https://github.com/OluwatobiAkintokun/PROJECT-SOCIAL-BUZZ/assets/137109080/f973fb0f-5853-424b-9b73-e1035d52fd34)


# Insights and Recommendation
* Upon analyzing the data, I have identified 16 distinct content categories. My findings confirm that the five most popular categories of posts are, in order of popularity: Animals, Science, Healthy eating, Technology, and Food.

* 'Animals' stands out as the leading category, amassing a total reaction score of 1,897. Within this category, there are 570 audio posts, 342 GIFs, 674 photos, and 311 videos. This indicates a strong affinity among the audience for animal related content.

* The presence of both 'Food' and 'Healthy Eating' in the top 5 is insightful, emphasizing the high engagement with food related content. Healthy eating, ranking just above food, suggests that the user base is tilted towards individuals who prioritize their health. Collaborating with Healthy Eating brands, influencers, restaurants, and relevant social media entities presents an opportunity to amplify favoured content, subsequently increasing user reactions.

* The inclusion of 'Science' and 'Technology' in the top 5 highlights a preference for informative content that offers learning opportunities. I recommend that the business should consider launching educational campaigns or series within the 'Science' and 'Technology' category to provide users with valuable and informative content. This aligns with user interests and is likely to garner higher engagement.

* The data reveals that January is the most common month for users to post content. This aligns with the seasonal trends of social media users, as they tend to reconnect with others after major calendar events like Christmas.

* The analysis of the sentiment paints a clear picture. A significant 84.64% of users express positive satisfaction, 8.71% remain neutral, and 6.65% express negative sentiments. Based on this data, I would make the following recommendations. (1) Capitalize on the huge positive sentiment by highlighting and promoting content that resonates with users. This can include positive user reviews, success stories, or uplifting content. (2) Pay attention to the 6.65% with negative sentiment. Investigate the reasons behind it, whether it's related to specific content, user experiences, or other factors. Take steps to address these issues to improve user satisfaction. (3) Explore the content that falls under the neutral sentiment category. Consider ways to make it more engaging or informative to potentially shift it towards a positive sentiment.

Dataset from theforage.com (Accessed: July 2023)
