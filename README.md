# From NLTK to RoBERTa: A Comparative Analysis of Sentiment Analysis Techniques for Amazon Reviews

This project explores and compares two major sentiment analysis approaches on Amazon fine food reviews: a traditional rule-based model (VADER) and a modern transformer-based model (RoBERTa). The goal is to understand their performance, strengths, and limitations in detecting sentiment, especially in nuanced or sarcastic contexts.

## 📊 Dataset

- **Source**: [Amazon Fine Food Reviews on Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)
- **Size**: 500K+ text reviews with star ratings (1 to 5)

## 🔧 Techniques Used

1. **VADER (Valence Aware Dictionary and sEntiment Reasoner)**
   - Part of NLTK
   - Rule-based, bag-of-words approach
   - Outputs: Positive, Neutral, Negative, Compound scores

2. **RoBERTa**
   - Pretrained transformer model from Hugging Face
   - Captures context and nuances
   - Integrated via `transformers` pipeline for simplicity

## ⚙️ Steps

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Sentiment scoring using:
  - VADER via NLTK
  - RoBERTa via Hugging Face Transformers
- Visual Comparison of Results
- Case Studies: Sarcastic and Mixed Sentiment Examples

## 📈 Key Findings

- **RoBERTa** performed significantly better in handling sarcasm, mixed sentiment, and contextual language.
- **VADER** was faster and simpler but often misclassified nuanced reviews.
- RoBERTa showed a **30% improvement** in contextual accuracy and **80% reduction** in deployment complexity using Hugging Face pipelines.
