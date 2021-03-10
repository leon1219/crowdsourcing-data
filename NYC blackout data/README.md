NYC blackout of July 2019 
These data files were used to support the findings in the case study of the NYC blackout of July 2019 in the paper "Social Media Data sourcing for Sudden-onset Hazard Appraisal."

Document 1. tweet_data_ID.dox
It contains the tweet IDs for both retweets and tweets related to NYC blackout (189,709 records). The original dataset downloaded with the search terms including “power outage,” “blackout,” and “power cut”  in the date range from July 13 to July 15 2020. These data were stored in JavaScript Object Notation (.json) files, which were then converted to Excel (.xlsx) files for subsequent processing. The original dataset contains a total number of 315,500 records. However, there is no guarantee that these retrieved tweets were related to the Manhattan blackout. To deal with this issue, location-related terms including “New York,” “NY,” “NYC,” “Manhattan,” and “Time Square” were used for a second round of filtering and cleaning work . This filtering process reduced the data size from 315,500 to 189,709 records with the timeline from 6:47 pm on July 13 to 8:00 pm on July 15 (EST). 

Document 2. sentiment_accumulative.xlsx
This file containes the results of accumulative sentiment score for the study period.

Document 3. sentiment_average.xlsx
This file calculates the senitment average score for every 10 minutes during the first 5 hours of NYC blackout occured. 

Document 4. sentiment chaneg_ID.dox
This document mainly treats the incorret tweets that were classified by Waston NLP API. To improve the accuracy, we munually adjusted the tweets containes in this file. 

Document 5. nyc_blackout.twb
Tableau file used to creates Figure 4 in the paper.


Note: The training and testing datasets applied in this study included "processed" tweet messages. We suspect that the Twitter policy might not allow us to directly share those information. These datasets could be available upon reasonable requests for the authors of this PNAS paper.
