# Social-Media-Sentiment-Analysis
This is my Third internship project at Next24tech Technology and Services. This project deals with the Social-Media-Sentiment-Analysis using data analytics and ML algorithm.
This is the sentiment140 dataset.
It contains 1,600,000 tweets extracted using the twitter api . The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment .
It contains the following 6 fields:

target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)
ids: The id of the tweet ( 2087)
date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
flag: The query (lyx). If there is no query, then this value is NO_QUERY.
user: the user that tweeted (robotickilldozr)
text: the text of the tweet (Lyx is cool)

### Steps for Sentiment Analysis:
1. **Preprocess the Data**:
   - Remove unnecessary columns (e.g., timestamp, query info).
   - Focus on the tweet text and the sentiment label.

2. **Text Cleaning**:
   - Convert text to lowercase.
   - Remove URLs, special characters, punctuation, and numbers.
   - Handle mentions (e.g., `@username`) and hashtags.
   - Tokenization (splitting the tweet into words).
   - Remove stopwords (common words like "the", "and", etc., that don't contribute to sentiment).
   - Stemming or Lemmatization (reducing words to their base form).

3. **Feature Extraction**:
   - Use **Bag of Words (BoW)**, **TF-IDF**, or **Word Embeddings** (e.g., Word2Vec, GloVe) to convert text into numerical format.

4. **Sentiment Classification**:
   - Train a sentiment classifier using algorithms like **Logistic Regression**, **Naive Bayes**, **Support Vector Machines (SVM)**, or **Deep Learning** models (e.g., **LSTM**, **BERT**).
   - The label in the dataset (column 0) will act as the target for training.

5. **Model Evaluation**:
   - Split the data into training and test sets (e.g., 80/20 split).
   - Evaluate the model using metrics such as **accuracy**, **precision**, **recall**, and **F1-score**.

6. **Tuning & Optimization**:
   - Perform hyperparameter tuning (e.g., using Grid Search or Random Search) to improve model performance.
   - Consider using **ensemble methods** (e.g., Random Forest, Gradient Boosting) for better accuracy.
