# SentimentAnalysisSocialMedia
Sentiment analysis of social media posts on X (created July 2023).

This project was created on July 20, 2023, as part of the Cisco Career Exploration Program. Used pandas, numpy, matplotlib, scikit-learn, and seaborn for vectorization, logistic regression, and analysis of social media posts. Created a logistic regression classifier that predicts indicators of depression in social media text, trained on a labeled dataset of tweets.

## Dataset

- **Source:** [Sentimental Analysis for Tweets](https://www.kaggle.com/datasets/gargmanas/sentimental-analysis-for-tweets) (Kaggle)
- **Size:** 10,314 tweets
- **Labels:** Binary — 0 (no depression indicator) / 1 (depression indicator)
- **Split:** 80% train / 20% test

## Pipeline

1. **Data loading** — loading .csv file using pandas
2. **Text cleaning** — removing URLs and special characters
3. **Feature extraction** — TF-IDF vectorization to convert raw text into numerical features
4. **Model training** — scikit-learn `LogisticRegression`
5. **Evaluation** — classification report with precision, recall, and F1-score

## Results

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0 (no depression) | 0.97 | 1.00 | 0.98 | 1,607 |
| 1 (depression) | 1.00 | 0.88 | 0.94 | 456 |
| **Overall accuracy** | | | **0.97** | **2,063** |
