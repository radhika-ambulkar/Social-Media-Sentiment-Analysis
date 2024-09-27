# Social-Media-Sentiment-Analysis
This is my Third internship project at Next24tech Technology and Services. This project deals with the Social-Media-Sentiment-Analysis using data analytics and ML algorithm.
The dataset contains 27,481 rows and 4 columns with the following structure:

- **Columns:**
  - `textID`: A unique identifier for each tweet (no missing values).
  - `text`: The full text of the tweet (1 missing value).
  - `selected_text`: A part of the tweet that reflects the sentiment (1 missing value).
  - `sentiment`: The sentiment of the tweet, labeled as either *positive*, *neutral*, or *negative* (no missing values).

### First Few Rows of the Dataset:
- Example 1: 
  - Text: "I`d have responded, if I were going"
  - Selected text: "I`d have responded, if I were going"
  - Sentiment: Neutral
- Example 2:
  - Text: "Sooo SAD I will miss you here in San Diego!!!"
  - Selected text: "Sooo SAD"
  - Sentiment: Negative

### Steps for Sentiment Analysis:

1. **Data Cleaning:**
   - Handle missing values in the `text` and `selected_text` columns.
   - Remove unwanted characters, stop words, and punctuation from the `text`.

2. **Text Preprocessing:**
   - Tokenization: Break down the text into words or tokens.
   - Lemmatization/Stemming: Convert words to their base forms.
   - Convert all text to lowercase for uniformity.

3. **Label Encoding:**
   - Map the `sentiment` labels to numeric values, e.g., Positive = 1, Neutral = 0, Negative = -1.

4. **Feature Extraction:**
   - Use techniques like Bag of Words (BoW) or TF-IDF (Term Frequency-Inverse Document Frequency) to convert text data into numerical form.

5. **Model Building:**
   - Choose a machine learning algorithm (e.g., Logistic Regression, Naive Bayes, or Random Forest) to train a sentiment classification model.

6. **Model Training:**
   - Split the dataset into training and test sets.
   - Train the model using the extracted features and sentiment labels.

7. **Model Evaluation:**
   - Evaluate the model using metrics like accuracy, precision, recall, F1-score, and confusion matrix.

8. **Tuning and Optimization:**
   - Optimize the model using techniques such as cross-validation and hyperparameter tuning.
