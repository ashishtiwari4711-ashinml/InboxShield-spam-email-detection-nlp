# InboxShield-spam-email-detection-nlp

 *NLP Spam Email Detection System*

# Project Overview

This project builds a Natural Language Processing (NLP) based spam detection system

The goal is to automatically classify emails/messages as:

Spam

Ham (Not Spam)

Designed to replace fragile rule-based filters with machine learning models

Focuses on real-world problems such as:

Phishing emails

Promotional spam

Unwanted automated messages

# Business Problem

Email platforms face increasing volumes of:

Spam

Phishing attempts

Promotional noise

Current challenges:

Manual moderation does not scale

Rule-based filters are easily bypassed

Spam tactics constantly evolve

User trust decreases due to unwanted emails

# Solution:

Build an NLP-driven ML system that:

Learns from historical messages

Automatically flags spam in real time

Minimizes false positives

# Machine Learning Task

Type: Supervised Learning

Category: Text Classification

Target Variable: Spam / Ham

# Dataset

Dataset contains labeled email/text messages:

Message content

Spam indicator

Data Type

Unstructured text data

Binary classification labels

# Text Preprocessing Pipeline

Implemented using NLTK + Regex + Python

Cleaning Steps

Converted text to lowercase

Removed special characters using regex

Removed numbers

Tokenized text (WhitespaceTokenizer)

Removed stopwords

Lemmatized words using WordNetLemmatizer

# Feature Extraction

Used TF-IDF Vectorization

Converts cleaned text into numerical vectors

Captures:

Word importance

Frequency patterns

TF-IDF helps emphasize meaningful words while reducing noise.

⚙ Models Implemented

Two machine learning classifiers were trained:

# Multinomial Naive Bayes

Probabilistic classifier

Works well with TF-IDF features

Lightweight and fast

Common baseline for NLP tasks

Used to provide:

Initial benchmark

Comparison point

# Support Vector Machine (LinearSVC)

Linear Support Vector Classifier

Designed for high-dimensional text data

Finds optimal separating hyperplane between spam and ham

More powerful than Naive Bayes

# Model Evaluation

Used:

Classification Report

Precision

Recall

F1-score

Accuracy

Results:

Naive Bayes achieved ~97% accuracy

SVM achieved ~99% accuracy

SVM performed best with:

Higher precision

Lower false positives

Better generalization

# Libraries Used

Python

Pandas

NumPy

Matplotlib

Seaborn

NLTK

Scikit-learn

TextBlob

Regex

# Workflow

Load dataset

Clean raw text

Tokenize messages

Remove stopwords

Lemmatize words

Convert text → TF-IDF vectors

Split into training/testing sets

Train Naive Bayes

Train SVM

Compare performance

Generate classification reports

# Key Achievements

Built complete NLP preprocessing pipeline

Implemented two ML classifiers

Achieved up to 99% accuracy

Reduced spam misclassification

Demonstrated real-world NLP application

Created scalable automated filtering system

# Limitations

Dataset size limited

No deep learning models used

Does not handle concept drift

No real-time deployment

Language assumed to be English

# Future Improvements

Add deep learning (LSTM / BERT)

Handle multilingual spam

Deploy as API

Real-time email filtering

Continuous retraining

Add phishing URL detection

Integrate Explainable AI

# Practical Impact

Improves user experience

Reduces phishing risk

Saves manual moderation effort

Builds trust in email platforms

Provides scalable spam protection

# Conclusion

This project demonstrates how NLP combined with machine learning can effectively detect spam emails. Through proper preprocessing, TF-IDF feature extraction, and classifiers like Naive Bayes and SVM, the system achieves very high accuracy. The SVM model proves especially powerful for text classification. With further enhancements, this pipeline can be deployed as a production-grade spam filtering system.
