# Sentiment Analysis on Amazon Electronic Product Reviews

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview
This project performs **sentiment analysis** on Amazon Electronics product reviews to classify them into **Positive, Neutral, or Negative** categories. It helps businesses understand customer opinions and make data-driven decisions.

## Dataset
- Dataset: Amazon Electronics reviews  
- Source: [Kaggle Dataset](https://www.kaggle.com/datasets/saurav9786/amazon-product-reviews)  
- Size used: 10,000 reviews (sampled for memory efficiency)

## Project Steps
1. **Data Loading & Inspection**
   - Loaded dataset and checked columns.
   - Sampled 10,000 rows to reduce memory usage.
2. **Data Cleaning**
   - Removed missing values and irrelevant columns.
3. **Sentiment Labeling**
   - Converted `overall` ratings into sentiment categories:
     - 1–2 → Negative  
     - 3 → Neutral  
     - 4–5 → Positive
4. **Text Preprocessing**
   - Lowercasing, tokenization, stopword removal.
   - Vectorization using TF-IDF.
5. **Model Training**
   - Logistic Regression
   - Random Forest Classifier
6. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1 Score
   - Confusion matrix visualization
7. **Visualization**
   - Word Clouds for each sentiment category

## Key Findings
- Random Forest performed better than Logistic Regression.
- Positive reviews frequently mention words like *“good, excellent, love”*.
- Negative reviews include words like *“poor, bad, defective”*.

## How to Run
1. Clone the repository.
2. Open the notebook `Sentiment_Analysis.ipynb` in Kaggle or Jupyter.
3. Install required libraries: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `wordcloud`.
4. Run the notebook cells step by step.

## Conclusion
This project demonstrates how machine learning models can classify customer reviews efficiently, providing actionable insights for businesses.
