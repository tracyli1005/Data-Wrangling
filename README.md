# 🐶 Twitter Dog Rating Analysis with Image Prediction

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![Data](https://img.shields.io/badge/Dataset-Twitter%20Dog%20Ratings-green)](https://raw.githubusercontent.com/udacity/new-dand-advanced-china/master/%E6%95%B0%E6%8D%AE%E6%B8%85%E6%B4%97/WeRateDogs%E9%A1%B9%E7%9B%AE/image-predictions.tsv)

This Jupyter Notebook analyzes Twitter data focused on dog ratings and image predictions. The project cleans raw social media data, explores dog breed classifications, and visualizes key insights about how users rate and categorize dogs on Twitter.

---

## 📂 Project Overview
&zwnj;**Objective**&zwnj;:  
Clean and analyze Twitter data to uncover patterns in dog ratings (`rating_numerator/denominator`), breed classifications, and user interactions.

&zwnj;**Datasets Used**&zwnj;:
1. `twitter-archive-enhanced.txt`: Raw Twitter metadata containing:
   - `tweet_id`, `text`, `timestamp`
   - Dog ratings (`rating_numerator`, `rating_denominator`)
   - Dog attributes (`doggo`, `pupper`, `puppo`, `floofer`)
   - User-assigned dog `name`
2. &zwnj;**Image Prediction Data**&zwnj;: Downloaded from [external URL](https://raw.githubusercontent.com/udacity/new-dand-advanced-china/master/%E6%95%B0%E6%8D%AE%E6%B8%85%E6%B4%97/WeRateDogs%E9%A1%B9%E7%9B%AE/image-predictions.tsv) containing breed predictions from tweet images.

---

## 🔍 Key Analysis Steps

### 1. Data Collection & Cleaning
- 🛠️ Imported raw Twitter data and image prediction tables
- 🧹 Handled missing values and inconsistencies in `rating_numerator` (e.g., non-numeric values)
- 🐕 Standardized dog lifecycle stages:
  - `doggo` (adult dog), `pupper` (puppy), `puppo` (young pup), `floofer` (fluffy dog)
- 🔄 Merged datasets on `tweet_id` for unified analysis

### 2. Exploratory Analysis
- 📊 &zwnj;**Rating Distribution**&zwnj;:
  - Calculated normalized ratings (`rating_numerator/denominator`)
  - Identified outlier ratings (e.g., "177/10" for viral dog posts)
- 🖼️ &zwnj;**Breed Prediction Analysis**&zwnj;:
  - Compared user-assigned dog `name` vs. image prediction results
  - Top 3 predicted breeds per image (confidence scores included)
- 📅 Temporal trends in dog-related tweets

### 3. Visualization
- 📈 Histograms of normalized ratings
- 🐩 Bar charts for most common dog breeds (user-labeled vs. image-predicted)

---

## 🚀 Quick Start
1. &zwnj;**Clone the repository**&zwnj;:
   ```bash
   git clone https://github.com/tracyli1005/Twitter_Dog_Rating
