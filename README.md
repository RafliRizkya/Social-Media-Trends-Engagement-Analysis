# Social-Media-Trends-Engagement-Analysis

This repository contains an exploratory data analysis and machine learning project focused on identifying patterns and key factors that influence **engagement rate** in social media content. The analysis combines clustering, feature importance extraction from supervised models, and actionable insights to improve content strategy.

## 📊 Objective

To analyze social media content performance, especially how views, likes, comments, and shares affect engagement rate levels. The goal is to:
- Understand which features influence high engagement
- Group posts based on engagement patterns
- Provide actionable strategies for content improvement

## 📁 Dataset

This project uses a dataset sourced from Kaggle titled **"Viral Social Media Trends and Engagement Analysis"**, which can be accessed via the following link:

🔗 [Kaggle Dataset - Viral Social Media Trends and Engagement Analysis](https://www.kaggle.com/datasets/atharvasoundankar/viral-social-media-trends-and-engagement-analysis/discussion?sort=hotness)

## 🧠 Methods Used

### 1. **K-Means Clustering**
Unsupervised technique to cluster posts into 3 levels:
- **Cluster 0 (Low ER):** High views, but low engagement
- **Cluster 1 (Medium ER):** Balanced views and engagement
- **Cluster 2 (High ER):** Low views, but very high likes, comments, and shares

These clusters are used as `Engagement_Rate_Level` for supervised modeling.

### 2. **Feature Importance (Supervised Learning)**
We applied the following models:
- Decision Tree (with and without resampling)
- Random Forest (with and without resampling)
- XGBoost (with and without resampling)
- Logistic Regression (with and without resampling)

After evaluating all models, **Logistic Regression** was found to have the best overall performance for predicting engagement rate level. It provided clear interpretability and robust accuracy.

![Confusion Matrix](Logistic%20Regression%20-%20Confusion%20Matrix.png)

📌 Aggregated feature importance shows that:
- `Views` is the most important feature
- Followed by `Likes`, then `Shares`, and lastly `Comments`

![Feature Importance](All%20Model%20-%20Feature%20Importance.png)

## 🧪 A/B Testing Suggestion

Based on current findings:
- **Test version A:** Content that aims for virality (high views).
- **Test version B:** Content optimized for interaction (CTA comments, polls, shareable hooks).
- Measure engagement rate, not just raw views, as the key success metric.

## 📊 Power BI Dashboard

I uploaded a Power BI Dashboard in this repository to visualize the results interactively.

## 🧑‍💻 Author

Rafli Rizkya Sakti Nugraha  
📎 [LinkedIn](https://www.linkedin.com/in/raflirzkyaa/)  
📬 For collaboration: raflirsn15@gmail.com  
