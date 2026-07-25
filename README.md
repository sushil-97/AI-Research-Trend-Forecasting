# AI-Research-Trend-Forecasting

# AI Research Trend Forecasting

This repository contains an end-to-end data science project aimed at identifying and predicting trends in Artificial Intelligence research using the OpenAlex dataset.

## 📌 Project Overview
The goal of this project is to understand how research topics evolve over time and to forecast their future prevalence. We use Natural Language Processing (NLP) to cluster research papers and Machine Learning (ML) to predict publication volumes for the year 2025.

## 🛠️ Tech Stack
- **Topic Modeling**: [BERTopic](https://github.com/MaartenGr/BERTopic) (Transformer-based clustering)
- **Data Handling**: Pandas, NumPy
- **NLP**: NLTK (Lemmatization, Stopword removal)
- **Machine Learning**: Scikit-Learn (Linear Regression, Random Forest), XGBoost
- **Visualization**: Matplotlib, Seaborn

## 📊 Key Methodology
1. **Data Preprocessing**: Combined paper titles and topic metadata into a lemmatized text corpus.
2. **Clustering**: Identified 3 primary research pillars: *Material Science & ML*, *Healthcare & AI*, and *Explainable AI (XAI)*.
3. **Impact Analysis**: Analyzed the Pearson correlation between publication age and citation counts.
4. **Forecasting**: Developed a simple **Ensemble Model** (averaging Linear Regression, Random Forest, and XGBoost) to predict 2025 paper volumes.

## 📈 Results & Insights
- **Topic Shift**: Historical data shows a move from foundational Material Science research (2015-2017) toward specialized Healthcare AI applications.
- **Forecast**: Healthcare AI is projected to be the most resilient topic in 2025 (~1.18 papers in the current sample).
- **Model Performance**: The ensemble approach achieved an $R^2$ score between 0.77 and 0.91, providing a robust balance between bias and variance.

## 🚀 How to Run
1. Clone the repository.
2. Ensure you have the required libraries installed: `pip install bertopic xgboost scikit-learn nltk`.
3. Open and run the Jupyter/Colab notebook to reproduce the results.
