# Twitter Sentiment Analysis using NLP

This project leverages the Twitter API and Natural Language Processing (NLP) to perform sentiment analysis on tweets related to any topic specified by the user. The goal is to determine the sentiment of each tweet as positive, negative, or neutral based on its content.

## Key Features:
- **Tweet Fetching:** Utilizes the Twitter API to fetch a user-specified number of tweets on any given topic.
- **Text Preprocessing:** 
  - **Stemming & Lemmatization:** Reduces words to their root forms.
  - **Stop Words Removal:** Eliminates common words that do not contribute to sentiment (e.g., "and," "the").
  - **Text Formatting:** Cleans and formats the tweet text for analysis.
- **Sentiment Analysis:** 
  - **Polarity Calculation:** Uses TextBlob to calculate the sentiment polarity of each tweet.
  - **Classification:** Based on the polarity, tweets are classified as positive, negative, or neutral.
- **Model Implementation:**
  - **Logistic Regression:** Achieves an accuracy of **82.13%**.
  - **Naive Bayes Classifier:** Achieves an accuracy of **78.37%**.
  - **Random Forest Classifier:** Achieves an accuracy of **84.64%**.

## Technologies Used:
- **Python:** The primary programming language used for this project.
- **Tweepy:** A Python library to interact with the Twitter API.
- **NLTK & TextBlob:** Libraries used for text processing and sentiment analysis.
- **Scikit-learn:** Used for implementing machine learning models such as Logistic Regression, Naive Bayes, and Random Forest.

## How It Works:
1. **Fetch Tweets:** The application fetches tweets related to the user-specified topic using the Twitter API.
2. **Preprocess Text:** The fetched tweets are cleaned and preprocessed using NLP techniques, including stemming, lemmatization, and stop words removal.
3. **Analyze Sentiment:** The sentiment of each tweet is analyzed using the TextBlob library, classifying it as positive, negative, or neutral based on the calculated polarity.
4. **Model Training & Prediction:** The preprocessed tweets are then fed into three different classifiers—Logistic Regression, Naive Bayes, and Random Forest—to predict sentiment, with accuracy scores of 82.13%, 78.37%, and 84.64% respectively.

## Results:
- The Random Forest Classifier provided the best accuracy at **84.64%**.
- Logistic Regression and Naive Bayes also performed well, with accuracies of **82.13%** and **78.37%** respectively.

This project demonstrates how NLP and machine learning techniques can be applied to social media data to extract valuable insights, such as public sentiment on various topics.
