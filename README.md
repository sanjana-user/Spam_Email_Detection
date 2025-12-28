# Spam_Email_Detection

# **Problem Statement:**

Spam email can contain security risks, take up storage thereby reducing productivity. This project focuses on building a machine learning based spam detection system that classifies emails as spam or legitimate using natural language processing techniques.

# **Dataset:**

The dataset is taken from Kaggle, which contains labeled email messages classified as spam or non-spam (ham). Each record includes the raw email text along with its corresponding label.

- Rows: 5572
  
- Features: Category, Message
  
- Target Variable: Category (Spam/ Ham)
   
# **Tools:**

Pandas

Numpy 

Scikit Learn

Natural Language Tool Kit

String

# **Approach and Methodology:**

## **a) Data Preprocessing:**

Removed all the null values. 

Duplicates are dropped.

## **b) Count Vectorizer:** 

- The punctuations are removed using the string.punctuation library.

- The stopwords like is, the, in, and etc (which are present in most of the mails) are removed.

- The clean words are collected under each email, and kept in a bag of words. 

## **c) Train Test split:**

- The data is split into training and testing data using the Scikitlearn function, train_test_split().

- Training the data using the Naive Baye’s Classification model, a test data accuracy of up to 95.7% is obtained.

## **d) Feature Importance:**

Creating a new table, with features and their importances (calculated using feature_importances_ attribute of random forest), a bar graph visualised their importances.

# **Models used:**

## **Bag of Words:**
A model that creates a matrix that has the frequency of each word stored for every email (rows) and every word (columns) ignoring the order. (text to vector conversion).

## **Naive Baye’s Classifier:**
Similar to the classic naive baye’s probability calculation, the probability of occurrence of a word given that it is spam/ham is noted for the training data and used to predict the test data.

# **Evaluation Metrics:**

## **Confusion Matrix:**
It compares the model predicted values and the actual known values in a tabular way. 
Confusion Matrix for our model:
[ [870, 33],

  [11,  118]  ]
  
## **Accuracy:** 
It calculates the proportion of correct predictions. For example, if a model correctly predicts 90 out of 100 instances, the accuracy is 0.9. Our model’s accuracy is 95.7%.

# **Insights:**

-The model was able to correctly identify spam and non-spam emails with high reliability.

-Text preprocessing and vectorization play a key role in improving classification performance.

-The model generalized well to unseen email messages.

# **How to run the project:**

-Download or clone the repository.

- Open the project folder.

- Open the Jupyter Notebook file (.ipynb).

- Run all the cells from top to bottom.

# **Project Structure:**

├── set_spam.csv        # Dataset used in the project

├── Spam.detection.ipynb      # Jupyter Notebook with full code

├── README.md          # Project explanation
