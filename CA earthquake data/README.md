### Ridgecrest earthquake sequence of July 2019

These data files were used to support the findings in the case study of the Ridgecrest earthquake sequence of July 2019 in the paper "Social Media Data for Sudden-onset Hazard Appraisal."

#### Document 1. tweet_data.xlsx
It contains the tweet IDs for both retweets and tweets related to earthquake daamge (51,043 records). It is worth noting that only original tweets were used for the analysis in the paper. The original dataset downloaded with the search term "earthquake" in the date range from July 4 to July 10, 2019 can be available upon reasonable request for non-commercial research purposes. The original dataset contains 1,482,937 English records. 

#### Document 2. damage_filter_seeds.docs
These filter seeds were used to identify damage-related tweets. Different forms of these filter seeds were considered (e.g., damage, damages, and damaged). 

#### Document 3. false_filter_seeds.xlsx
Phrases containing damage-related words may not indicate “real” earthquake damage of impacts, such as “scared me to death,” “broke my heart,” “crack me up,” and “kill my sleep.” This library of filter seeds was used to remove tweets not implying “real” status of damage (i.e., “false damage” indicators). This filtering process resulted in a set of presumptive “real” damages related tweets containing 51,043 records.

#### Document 4. tweet_volume_words.xlsx
This document mainly tracks two sets of tweets in the study based on 1,482,937 English records: original tweets created by a user, and “retweets” forwarded by a second user, and the average words-per-tweet and the average characters-per-tweet in every 30-minute interval. This data file was used to create Figure 1 in the paper. 

#### Document 5. damage_classification_result.xlsx
This document contains the damage classifications using the TF-IDF + RF pipeline. It also contains the county information based on the location extraction using the Standford Name Entity Recognition (NER) API. The NER tool applied in this study was built based on a 3-class model that can recognize location, person, and organization from a text. https://stanfordnlp.github.io/CoreNLP/ner.html.

#### Document 6. county_damage.xlsx
The mean damage level of each county group was computed and assigned as the estimated damage level for that county. This document was used to generate Figure 2a in the paper. 

#### Document 7. MMI_intensity.xlsx
This dataset contains the information from the USGS Shakemap for the mainshock event https://earthquake.usgs.gov/earthquakes/eventpage/ci38457511/pager. In the paper, Figure 2b shows a map of the county-level averaged MMI based on this dataset. 

#### Document 8. ca_earthquake.twb
Tableau file creates Figure 1 and Figure 2 in the paper.  

#### Document 9. tfidf_classifiers.ipynb; Document 10. embedding_lstm.ipynb; Document 11. classifiers_performance.docx
Several text classification pipelines were built to classify each damage-related tweet into one of the corresponding damage levels. The text classification pipeline was constructed in two steps: (1) text vectorization, and (2) multi-class classification. 

Two popular text vectorization approaches were applied including Term Frequency-Inverse Document Frequency (TF-IDF) and word embedding methods. Word embedding methods applied in this study include FastText and GloVe. 

Classifiers applied in this study include: Random Forest (RF), Naïve Bayes (NB), Support Vector Machine (SVM), Logistic Regression (LR), and Long Short-Term Memory (LSTM). RF, BB, SVM, and LR are simple and well-developed machine learning classifiers and can be used in conjunction with the TF-IDF text vectorization method. Models using these four classifiers combined with the TF-IDF technique were constructed based on the scikit-learn python library (Document 9). An Bidirectional LSTM is used for text classification in conjunction with word embeddings (Document 10). 

The training dataset was built based on our manual classification for 1,771 samples from this Ridgecrest earthquake dataset and 727 samples from a public earthquake dataset https://crisisnlp.qcri.org/lrec2016/lrec2016.html. The final combined training dataset included 417 level 0 damage samples, 299 level 1 damage samples, 1,190 level 2 damage samples, and 592 level 3 damage samples. However, to deal with the imbalance, we applied a simple text augmentation technique called Easy Data Augmentation (EDA) https://github.com/jasonwei20/eda_nlp. The augmented training dataset contained 1,251 level 0 damage samples, 1,196 level 1 damage samples, 1,190 level 2 damage samples, and 1,184 level 3 damage samples. 

The testing dataset was built based on our manual classification for a random set of 800 samples from the Ridgecrest earthquake dataset. Metrics including Recall, Precision, F1-score, and Accuracy were applied to select the model. The performance of each pipeline was listed in Document 11. 

#### 













