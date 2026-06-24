# Sentiment Analysis on Amazon Product Reviews

## Project Overview

This project develops a machine learning-based sentiment analysis system capable of classifying Amazon product reviews into Positive, Neutral, and Negative categories.

The objective is to transform unstructured customer feedback into actionable insights using Natural Language Processing (NLP) and supervised machine learning techniques.

Developed as part of the Optimus Automate Machine Learning Internship Program.

---

## Business Problem

Online marketplaces receive thousands of customer reviews daily. Manually analyzing customer feedback is time-consuming and inefficient.

This project automates the process by predicting the sentiment of customer reviews, helping organizations:

* Monitor customer satisfaction
* Identify negative feedback quickly
* Improve products and services
* Support data-driven decision making

---

## Dataset

**Dataset:** Amazon Fine Food Reviews

The dataset contains customer reviews, ratings, and product feedback collected from Amazon.

Key attributes used:

* Review Text
* Review Score

Sentiment labels were generated from review ratings:

| Rating | Sentiment |
| ------ | --------- |
| 4-5    | Positive  |
| 3      | Neutral   |
| 1-2    | Negative  |

---

## Project Workflow

### 1. Data Preprocessing

The following preprocessing steps were applied:

* Missing value handling
* Lowercasing
* Removal of punctuation
* Stopword removal
* Text cleaning

### 2. Feature Engineering

Text data was converted into numerical features using:

* TF-IDF Vectorization
* Unigrams and Bigrams
* Maximum Features: 10,000

### 3. Model Development

Two machine learning models were trained and evaluated:

#### Model 1: Multinomial Naive Bayes

A probabilistic classifier commonly used in text classification tasks.

#### Model 2: Linear Support Vector Machine (SVM)

A high-performance classification algorithm widely used in industrial NLP applications.

---

## Model Evaluation

Performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### Results

| Model                   | Accuracy |
| ----------------------- | -------: |
| Multinomial Naive Bayes |   81.64% |
| Linear SVM              |   86.06% |

### Best Performing Model

Linear SVM achieved the highest classification accuracy and was selected as the final model.

---

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-Learn
* Matplotlib
* Seaborn
* Joblib

---

## Repository Structure

```text
Sentiment Analysis on Product Reviews/
│
├── Amazon_Product_Review_Sentiment_Analysis.ipynb
├── sentiment_model.pkl
├── tfidf_vectorizer.pkl
├── requirements.txt
└── README.md
```

---

## Future Improvements

* Deep Learning Models (LSTM, GRU)
* Transformer Models (BERT)
* Real-Time Sentiment Prediction API
* Web-Based Dashboard
* Model Deployment using FastAPI

---

## Author

Muhammad Abdullah Awan
