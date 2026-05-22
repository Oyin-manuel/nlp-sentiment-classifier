# 💬 Social Media Sentiment Classifier

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-red?logo=scikit-learn)](https://scikit-learn.org/)
[![NLP](https://img.shields.io/badge/NLP-TF--IDF-purple)]()

## 📌 Business Overview
Modern businesses generate massive amounts of unstructured text data through social media and customer reviews. Extracting actionable insights from this text is critical for brand monitoring. This project builds an end-to-end **Natural Language Processing (NLP)** pipeline to automatically classify raw text into structural sentiment categories (Positive, Negative, Neutral).

## ⚙️ Technical Approach
* **Text Preprocessing:** Engineered a custom regex cleaning pipeline to remove URLs, mentions, hashtags, and punctuation. Applied stopword removal and tokenization to reduce noise.
* **Feature Extraction:** Transformed text into a numerical matrix using a **TF-IDF Vectorizer** (Term Frequency-Inverse Document Frequency), capturing up to 3,000 top unigrams and bigrams to preserve context (e.g., "beautiful day" vs "terrible morning").
* **Predictive Modeling:** Trained and evaluated multiple classification models, specifically comparing **Naive Bayes** against **Logistic Regression**. 

## 📊 Key Findings & Business Impact
* **Model Performance:** The Naive Bayes classifier achieved a strong accuracy of **~79%** across the multi-class problem.
* **Class Optimization:** The model excelled at identifying the 'Positive' class (F1-Score: 0.86). The analysis also highlights the challenges of class imbalance regarding the 'Neutral' class, providing a roadmap for future dataset augmentation.
* **Interpretability:** Extracted log probabilities to visualize the top predictive keywords per class, allowing stakeholders to see exactly *why* the model makes a decision.

## 🧰 Tech Stack
* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `scikit-learn`, `re` (Regex), `matplotlib`, `seaborn`

## 🚀 How to Run Locally
1. Clone this repository.
2. Install dependencies.
3. Run `sentiment_analysis_nlp.ipynb` to view the text cleaning pipeline and model evaluation metrics.
