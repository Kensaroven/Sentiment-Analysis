# Sentiment-Analysis

## Academic Project

#### Some of the key questions to answer are:

1. What are the issues with given text data and discuss what type of pre-processing would be required?

2. Discuss a few exploratory data analyses (EDA) and trend analyses that can be carried out on the given text data? 

3. Perform feature extraction and feature selection for sentiment analysis.

4. Develop a Bayes-supervised learning model to predict the sentiment of a review.  

5. Discuss the sampling strategy you would be using for the given dataset. What will be your strategy for dealing with the imbalanced dataset? 

6. Discuss lexicon-based approaches to predict the sentiment of a review. 

7. Develop an appropriate model to predict the emotion of a review. 

Answer: Some of the lexicon-based approaches we have used above in predicting the sentiment of a review is mentioned below.  
- AFINN Lexicon (Affective Norms for English Words): It is a simple lexicon-based approach for sentiment analysis and consists of a list of words that have been manually assigned a polarity score. This score is a numerical value indicating the sentiment or emotion associated with that word. Each word is given a score ranging from -5 (most negative) to 5 (most positive), with 0 being neutral score. In our text above, AFINN score was assigned to a total of 4641 words. Here, we see that about 4060 positive reviews and about 581 negative reviews.

- Text Blob - It is a pre-trained sentiment analysis model that can be used to classify the sentiment of text as positive, negative, or neutral. It uses a rule-based approach to assign polarity scores to individual words and then aggregates the scores to determine the overall sentiment of the text. The overall results, as shown above, of the confusion matrix and classification results are found to be better than previous ones. 

- Vader Lexicon (Valence Aware Dictionary and sEntiment Reasoner) - It is a lexicon and rule-based sentiment analysis tool specifically designed for social media texts. It takes into account the nuances of social media language, such as the use of slang, emojis, and capitalization, in order to provide accurate sentiment analysis. Vader assigns each word in the text a polarity score, which ranges from -1 (most negative) to 1 (most positive), and also provides a compound score, which represents the overall sentiment of the text. The compound score is a normalized, weighted composite score that ranges from -1 to 1, where values above 0.05 are generally considered positive, values below -0.05 are considered negative, and values in between are considered neutral. The specific results of Vader Lexicon are shown above.


8. What are the comprehensive insight from this mining process?

Answer: A large majority of the people associate positive emotions with ISKON, this could also be a reflection fo ISKON's charitable activities outside of temples or even the religious, respectful aspect of deity worship. We can also see that the second major emotion is anticipation. This makes sense as well; ISKON is an extremely popular worldwide movement, which generates curiousity in its potential visitors. 

Suprisingly, this is closely followed by anger. On closely reviewing the Question 4 output where we use a Bayes-supervised learning model for sentiment review, we can see the common theme in negative reviews revolves around the commercialization of the temple complex which many devotees feel takes away from true worship or the humble atmosphere of a supposed temple.

Lastly, we can see that the negative emotions associated with ISKON are pretty low as compared to the positive emotions however, we can still comb through these reviews to get insights on how the temple can improve it's visitor experience.

9. What should be the strategy for the deployment of the model?

Answer: The most crucial step for the deployment of this model is data collection as currently the temple is using less-than-adequate and unreliable ways of data collection. In order to encourage people to fill in more feedback during the visit to the temple, the temple can look into installing electronic kiosks which provide information about the temple as well as allow feedback and suggestions. Additionally, we should build an automated pipeline to periodically scrape all popular social media websites for any relevant reviews instead of having the IT team manually search for them.
Following the data collection process, a pipeline needs to be setup for data pre-processing to clean the data and make it ready for analysis for the future steps.

Lastly, this data can be used to train the model and prepare it for future feedback review with greater accuracy.

Further down the line, this model can be extended to single out negative reviews and do a deeper textual analysis to find the core complaints or suggestions that visitors have for the temple which can then be converted into actionable insights.

Also, the IT team for ISKON needs to be trained for the upkeep and maintainence of the model inorder to make the process faster and more reliable.
