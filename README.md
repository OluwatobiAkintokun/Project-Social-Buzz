# PROJECT-SOCIAL-BUZZ

# BUSINESS QUESTION

This project revolves around the examination of 'Social Buzz,' a company that is progressively evolving into a global unicorn enterprise. Their platform routinely receives an influx of over 100,000 posts daily, aggregating to a staggering 36,500,000 posts annually. Notably, this data is predominantly unstructured, rendering it complex to extract meaningful insights. The key focus of this analysis is to highlight the top 5 content categories within this datasets.

# DATASETS

There are 3 datasets provided for this analysis.
1.	Content Dataset – The Content dataset consists of the following column names: Content ID, User ID, Type, Category, and URL.
2.	Reactions Dataset - The Reactions dataset consists of the following column names: Content ID, User ID, Type, and Datetime
3.	Reaction Types Dataset- The Reaction Types dataset consists of the following column names: Type, Sentiment, and Score.
   
   Please see attached.
   
# DATA CLEANING

1.	I refined our datasets by removing unnecessary columns and rows that didn't pertain to the primary business question. This included the removal of the ‘URL’ and ‘User ID’ columns in the Content dataset, as well as the ‘User ID’ column in the Reactions dataset. Blank rows, which were not relevant to our analysis, were also removed from all three datasets.
2.	I standardized the column names across the datasets to ensure consistency. Specifically, I replaced the 'Type' column in the Content dataset with 'Content Type' and made the same adjustment in the Reactions and Reaction Types dataset, where 'Type' became 'Reaction Type'. 
3.	In addition, I removed quotation marks from ‘categories’ column in the Content dataset to maintain a uniform naming convention.
   
   Note: Data cleaning was done using Ms Excel.

  # DATA TRANSFORMATION 
1. I created a finalized dataset titled 'Clean Merged Dataset' by merging information from the Content, Reactions, and Reaction Types datasets. This merging process was executed using the ‘VLOOKUP’ formular within Ms Excel, with the Reaction Table serving as the base table.
![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/3f14427c-3c80-47dc-ab50-73cebaa8a54d)

2. In order to identify the top 5 categories, I computed the cumulative scores for each category by applying the 'SUMIF' formula in Microsoft Excel.
   
![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/d70af9fe-bee3-4345-97e0-38af499472f3)

3. See below Top 5 categories

![image](https://github.com/Tanpepper29/PROJECT-SOCIAL-BUZZ/assets/137109080/4e4dd04e-e690-4624-8985-9463c5da7147)





