# Twitter Sentiment Analysis Project 💬📊

A machine learning project focused on classifying sentiments in tweets by testing three models to determine the most reliable: **Support Vector Machine (SVM)**, **Logistic Regression Model (LGM)**, and **Naive Bayes (NB)**. This project aims to understand which model performs best on this dataset, with insights into model selection based on performance metrics.

## Project Overview

Sentiment analysis is an essential technique in natural language processing (NLP), commonly used for social media monitoring. By leveraging ML algorithms, this project identifies and classifies the sentiment expressed in tweets, categorizing them as positive, negative, or neutral.

### Models Tested
1. **Support Vector Machine (SVM)**
2. **Logistic Regression Model (LGM)**
3. **Naive Bayes (NB)**

### Results
- **Performance Comparison**:
  - **Test 1**: LGM (92%) > SVM (90%) > NB (89%)
  - **Test 2**: LGM (82%) > SVM (81%) > NB (80%)
- **ROC Curve**: Identical through the three models

- **Analysis**:
  The results indicate that Logistic Regression consistently outperforms SVM and Naive Bayes on this dataset. Logistic Regression's simplicity aligns with **Occam’s Razor**, which posits that simpler models are often effective, particularly when the dataset doesn’t require specific assumptions. Given our data’s lack of underlying assumptions, Logistic Regression’s straightforward nature allows it to achieve reliable results.

## Technologies Used 🛠️

- **Python**: Programming language for building, training, and testing ML models.
- **Libraries**:
  - **Scikit-Learn**: For implementing and evaluating machine learning models.
  - **Pandas**: For data manipulation and preprocessing.
  - **NumPy**: For numerical computing.
  - **Matplotlib**: For data visualization and plotting.
  - **WordCloud**: For visualizing common words in tweets.
  - **NLTK**: For natural language processing, tokenization, and text preprocessing.

---

## Project Flowchart

```plaintext
1. Import Necessary Dependencies
2. Read and Load the Dataset
3. Exploratory Data Analysis (EDA)
    └── Data Visualization of Target Variables
4. Data Preprocessing
    ├── Tokenization
    ├── Stemming
    └── Lemmatization
5. Splitting Data into Train and Test Sets
6. Transforming Dataset using TF-IDF Vectorizer
7. Define Evaluation Function
8. Model Building
    ├── Support Vector Machine
    ├── Logistic Regression Model
    └── Naive Bayes
9. Model Evaluation
