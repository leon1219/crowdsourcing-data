### Ridgecrest earthquake sequence of July 2019

These data files are used to support the findings in the case study of Ridgecrest earthquake sequence of July 2019 in the paper "Social Media Data for Sudden-onset Hazard Appraisal."

#### Document 1. tweet_data.xlsx
Contains the tweet IDs for both retweets and tweets related to earthquake daamge (51,043 records). It is worth noting that only original tweets were used for the analysis in the paper. The original dataset downloaded with the search term "earthquake" in the date range from July 4 to July 10, 2019 can be available upon reasonable request for non-commercial research purpose. The original dataset contains 1,482,937 English records. 

#### Document 2. damage_filter_seeds.docs
These filter seeds were used to identify damage-related tweets. Different forms of these filter seeds were considered (e.g., damage, damages, and damaged). 

#### Document 3. false_filter_seeds.xlsx
Phrases containing damage-related words may not indicate “real” earthquake damage of impacts, such as “scared me to death,” “broke my heart,” “crack me up,” and “kill my sleep.” This library of filter seeds was used to remove tweets not implying “real” status of damage (i.e., “false damage” indicators). This filtering process resulted in a set of presumptive “real” damages related tweets containing 51,043 records.

#### Document 4. tweet_volume_words.xlsx
This document mainly tracks two sets of tweets in the study based on 1,482,937 English records: original tweets created by a user, and “retweets” forwarded by a second user, and the average words-per-tweet and the average characters-per-tweet in every 30-minute interval. This data file was used to create Figure 1 in the paper. 

#### Document 5. damage_classification_result.xlsx
This coument contains the damage classifications using the TF-IDF + RF pipeline. It also contains the county information based on the location extraction using the Standford Name Entity Recognition (NER) API. The NER tool applied in this study was built based on a 3-class model that can recognize location, person, and organization from a text. https://stanfordnlp.github.io/CoreNLP/ner.html.

#### Document 6. county_damage.xlsx






