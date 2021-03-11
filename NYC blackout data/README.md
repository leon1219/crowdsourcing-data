### NYC blackout of July 2019 
These data files were used to support the findings in the case study of the NYC blackout of July 2019 in the paper "Social Media Data sourcing for Sudden-onset Hazard Appraisal."

#### Document 1. tweet_data_ID.dox
It contains 189,709 records of the tweet IDs for both retweets and tweets related to the NYC blackout. Retweets were not removed for the present study given that people who retweeted a tweet could possibly witness the same blackout event or hold the same feelings or thoughts as the original tweet. A tweet with more retweets also implies that the details described by the tweet for the Manhattan blackout was recognized by more people. 

The sentiment values were output by IBM Watson NLP tool https://www.ibm.com/cloud/watson-natural-language-understanding. We applied a sign function to simply treat all the negative sentiment as “-1”, neutral as “0”, and positive as “1.” 

#### Document 2. sentiment_accumulative.xlsx
This file contains the results of the accumulative sentiment score for the study period. This defined variable “accumulative sentiment” reflects the overall changes of sentiment and compensates for the effects of wild swings of sentiment resulting from low tweets volume in a short time interval. 

#### Document 3. sentiment_average.xlsx
This file calculates the average score of sentiment in every 10 minutes during the first 5 hours since NYC blackout hit the afflicted areas. 

#### Document 4. sentiment chaneg_ID.docx
This document mainly treats the incorrect tweets that were classified by Waston NLP API. When we tested the performance of the API tool using a random sample of 410 unique tweets, we found that a number of sentiments were wrongly output by the API possibly because the tool was not trained based on blackout-related word domain. To improve the accuracy of sentiment extraction, we manually adjusted the sentiment of these tweets contained in this file. This observation brings forward the potential necessity for either manual modifications in limited circumstances or the need to improve the sentiment results when a few widely retweeted tweets are incorrectly classified due to the limitations of the sentiment tools. 

#### Document 5. nyc_blackout.twb
Tableau file to create Figure 4 in the paper.
