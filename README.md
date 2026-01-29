# 🎵 TikTok Video Classification Project

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit_Learn-orange)
![Model](https://img.shields.io/badge/Model-XGBoost-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Project Overview
The goal of this project is to build a machine learning model that classifies TikTok videos as either **"Claim"** or **"Opinion"**. By distinguishing between these two categories, the platform can prioritize user reports more efficiently and mitigate the spread of misinformation.

This project follows the **PACE** (Plan, Analyze, Construct, Execute) framework to ensure a structured and rigorous data science workflow.

## ❓ Business Problem
TikTok users report videos that violate terms of service. Given the massive volume of daily uploads, manual review of every report is impossible.
* **Claims:** Factual assertions that can be verified (higher risk of misinformation).
* **Opinions:** Personal beliefs or thoughts (lower priority).

**Objective:** Develop a binary classification model to flag "Claim" videos for priority moderation.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn, XGBoost
* **Natural Language Processing:** CountVectorizer (for text feature extraction)

## 📂 Dataset
The dataset contains approximately 19,000 video records with the following key features:
* `claim_status`: Target variable (Claim vs. Opinion)
* `video_transcription_text`: Transcribed text from the video
* `video_view_count`, `like_count`, `share_count`: Engagement metrics

*> **Note:** The dataset is provided by Google & Coursera. Due to file size limits/licensing, the raw CSV file is not included in this repository.*

## 📊 Model Performance
Two ensemble learning models were trained and evaluated: **Random Forest** and **XGBoost**.

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| **Random Forest** | **99.5%** | **99.5%** | **99.5%** | **99.5%** |
| XGBoost | 99.2% | 99.4% | 99.1% | 99.3% |

**Champion Model:** The **Random Forest** model was selected as the champion model due to its superior Recall score, which is critical for minimizing false negatives (missing a potential violation).

## 🚀 Key Insights
1. **Engagement Matters:** The most predictive features were engagement metrics (`video_view_count`, `video_like_count`). Claim videos tend to have significantly higher engagement than opinion videos.
2. **Text Length:** Claim videos generally have longer transcription text compared to opinions.

## 💻 Getting Started
To run this project locally, follow these steps:

1. **Clone the repository**
   ```bash
   git clone [https://github.com/KULLANICI_ADIN/TikTok-Video-Classification-ML.git](https://github.com/KULLANICI_ADIN/TikTok-Video-Classification-ML.git)
