# Sentiment Analysis on 2019 Indonesia Election Tweets

## Background
This project aims to analyze the sentiment of tweets related to the 2019 Indonesia Election. Sentiment analysis plays a crucial role in understanding public opinion and attitudes towards political events, providing valuable insights for decision-making and public discourse.

## Goal
The primary goal of this project is to develop a sentiment analysis model that accurately predicts the sentiment (positive, negative, or neutral) of tweets regarding the 2019 Indonesia Election. By analyzing the sentiment expressed in tweets, we aim to gain insights into public perception and sentiment towards political events during the election period.

## Text Preprocessing
In this project, we performed extensive text preprocessing to prepare the tweet data for sentiment analysis. The preprocessing steps included:
1. **String Parsing:** Ensuring consistency by converting all tweets to string format.
2. **Split Hashtag:** Splitting camel case hashtags to improve readability.
3. **Lowercasing:** Converting all text to lowercase to standardize the text.
4. **Remove URL:** Eliminating URLs from the text data to remove irrelevant information.
5. **Remove HTML Tags:** Stripping HTML tags from the text data.
6. **Remove Numeric:** Replacing numeric values with their respective textual representation.
7. **Remove String Emoticon:** Removing string emoticons from the text.
8. **Remove Punctuation:** Removing punctuation marks from the text while retaining single quotes.
9. **Extract Emoji:** Replacing emojis with their textual descriptions.
10. **Remove Special Character:** Eliminating special characters from the text data.
11. **Remove 3 Repeating Characters:** Reducing repeating characters to a maximum of two consecutive occurrences.
12. **Remove Single Word:** Removing standalone single characters from the text.
13. **Stemming:** Applying stemming using the Sastrawi library to reduce words to their root forms.
14. **Remove Stopwords:** Initially intended to remove stopwords, but not executed due to the risk of losing contextual information.

## Exploratory Data Analysis (EDA)
The EDA revealed the distribution of sentiments (positive, negative, neutral) across different candidates (Jokowi, Prabowo, Maruf, Sandi) based on the tweet data.

## Dataset Creation
We created datasets for modeling by vectorizing the preprocessed tweet text using various techniques:
- Frequency-Based Vectorization: Count Vectorization and TF-IDF Vectorization
- Co-Occurrence Matrix
- N-Gram Vectorization
- Prediction-Based Vectorization: CBOW and Skip-gram Word2Vec models

## Modeling
We trained two models for sentiment analysis:
1. LSTM (Long Short-Term Memory) Neural Network
2. Random Forest Classifier

## Conclusion
In this project, using TF-IDF vectorization and the Random Forest model, we achieved an accuracy of 66% and an F1 score of 61% in predicting sentiment from tweets related to the 2019 Indonesia Election. The results demonstrate the effectiveness of the model in capturing public sentiment and providing valuable insights into the opinions and attitudes of the Indonesian population towards political events.
