## Data Descriptions

These data files are used to support the findings in the paper "Social Media Data for Sudden-onset Hazard Appraisal." (Lingyao Li, Michelle Bensi, Ma Zihui, Yu Wang, and Gregory B. Baecher).

Three recent hazard events were used as the basis for this study: (1) the Ridgecrest earthquake sequence of July 2019, (2) the Notre Dame Cathedral fire of April 2019, and (3) the New York City blackout of July 2019.

### 1. Ridgecrest earthquake sequence of July 2019
The Twitter Search API was used with a filtering word “earthquake” to scrape earthquake-related data from 4 July to 10 July, 2019. A library of words implying damage (e.g., “damage,” “injury,” “destroy,” and “crack.”) was developed and applied to filter damage-related tweets. The final dataset used for damage analysis included 51,043 tweets, in which 9,197 are original tweets. Retweets were removed for the analysis, assuming that an original tweet describing damage was likely to be a first-hand observation or report. 

### 2. Notre Dame Cathedral fire of April 2019
The Twitter search API with a search phrase “Notre Dame” was applied to download tweet data in the date range from April 15 to April 25, 2019. Twelve fire factors, as listed below, were selected to filter fire “reasoning” tweets. The resulting database included 50,202 records (1,533 tweets posted from verified users and 48,669 tweets posted from non-verified users) and was used to investigate public opinions regarding the causes of the fire incident. 

### 3. New York City blackout of July 2019
Key search terms including “power outage,” “blackout,” and “power cut” were used with Twitter search API to collect Twitter data from July 13 to July 15, 2020. Location-related words such as “New York,” “NY,” “NYC,” “Manhattan,” and “Time Square” were selected to filter data related to New York blackout. This filtering process resulted in a dataset of 189,709 records used for the sentiment analysis. 

According to the Twitter Developer Policy, https://developer.twitter.com/en/developer-terms/agreement-and-policy#id34, restrictions apply to the availability of Twitter data, which are used under Twitter license for the current study, so specific user information or tweets messages are not publicly available without the permission of Twitter Inc. The tweet IDs and User IDs are however available for non-commercial research purposes and attached in each folder. 

#### NOTE: The original datasets for Ridgecrest earthquake case and NYC blackout case downloaded with Twitter Search API were available in their folders. These tweet data can be used for non-commercial research purposes under Twitter policy.
