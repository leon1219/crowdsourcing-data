### Notre Dame Cathedral Fire of April 2019
These data files were used to support the findings in the case study of the Notre Dame Cathedral fire of April 2019 in the paper "Social Media Data for Sudden-onset Hazard Appraisal."

#### Document 1. tweet_data.xlsx
This spreadsheet contains the user IDs for both retweets and tweets related to users’ opinion on fire causes (50,202 records). The original dataset downloaded with the search term "Notre Dame" in the date range from April 15 to May 15, 2019 can be available upon reasonable request for non-commercial research purposes. The original dataset contains 9,115,833 records.

#### Document 2. sample_verification.xlsx
This spreadsheet contains the validation of the model using 565 tweets randomly selected from the dataset. Each tweet was manually classified into “oppose (-1),” “uncertain (0),” or “support (1)” in terms of the fire cause, and then the predicted opinion output by the model was compared with the manual label. 

#### Document 3. opinion_distribution.xlsx
This spreadsheet contains the result of opinion distributions for verified users and non-verified users. For each cause-opinion combination (e.g., {act of god: -1}), the total count is the sum of three counts because at most three fire factors can be identified in a single tweet (as shown in tweet_data.xlsx). 

#### Document 4. temporal_data.xlsx
This spreadsheet presents the time series data based on a 12-hour interval, including total tweet volume over time, tweet volume for non-verified users and verified users, percentages of top four fire causes collected from non-verified users and verified users, percentages of criminal and accidental causes from non-verified users and verified users. 


#### Document 5. word libraries.docx
This document includes all the word libraries that was used for cleaning datasets and the development of the text-parsing and lexicon-based rule model. 
