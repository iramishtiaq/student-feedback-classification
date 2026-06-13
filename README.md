Student Feedback Classification Using NLP and Machine Learning
Project Overview

This project focuses on automatically classifying student feedback as either Positive or Negative using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to analyze student course reviews and identify the sentiment expressed in the feedback.

The project demonstrates the complete NLP workflow, including text preprocessing, feature extraction, model training, evaluation, and result interpretation.

Dataset

The dataset contains student course reviews collected from an online learning platform. Each review is associated with a rating from 1 to 5.

To create a binary classification problem:

Ratings 1 and 2 were labeled as Negative
Ratings 4 and 5 were labeled as Positive
Rating 3 reviews were removed as they represent neutral sentiment

The original dataset was highly imbalanced, so a balanced dataset was created by randomly sampling positive reviews to match the number of negative reviews.

Final dataset size:

Positive Reviews: 4,720
Negative Reviews: 4,720
Total Reviews: 9,440
NLP Preprocessing Steps

The following preprocessing techniques were applied:

Lowercasing
Punctuation removal
Special character removal
Extra whitespace removal
Word tokenization
Sentence tokenization
Stopword removal
Stemming
Lemmatization

A final preprocessing pipeline using lemmatization was applied to all reviews before feature extraction.

Text Representation Techniques

The following text representation methods were explored:

Count Vectorizer (Bag of Words)
TF-IDF Vectorizer
N-Gram Models
Unigram
Bigram
Unigram + Bigram
Machine Learning Models

Three machine learning classifiers were trained and evaluated:

Naive Bayes
Logistic Regression
Support Vector Machine (SVM)
Results
Model Representation Accuracy
Naive Bayes Count Vectorizer 87.98%
Logistic Regression TF-IDF 89.14%
SVM TF-IDF 87.98%

Logistic Regression combined with TF-IDF achieved the best performance with an accuracy of 89.14%.

Visualizations

The project includes:

Class distribution analysis
Confusion Matrix
Word Clouds for Positive Reviews
Word Clouds for Negative Reviews
N-Gram vocabulary comparison
Key Findings
Text preprocessing significantly improved data quality.
TF-IDF produced better results than simple word counts.
Logistic Regression achieved the highest classification performance.
Word cloud visualizations helped identify common themes in student feedback.
Technologies Used
Python
Pandas
NumPy
NLTK
Scikit-learn
Matplotlib
Seaborn
WordCloud
Jupyter Notebook
Project Structure
StudentFeedbackClassifier/
│
├── data/
│ └── reviews.csv
│
├── notebook/
│ └── StudentFeedbackClassifier.ipynb
│
├── README.md

Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to automatically analyze student feedback and classify sentiment. The results show that machine learning models can effectively identify positive and negative reviews, providing useful insights that can support improvements in teaching and learning experiences.
