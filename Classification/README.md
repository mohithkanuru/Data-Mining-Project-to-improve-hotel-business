# Hotel Reviews Classification

## Overview

This repository contains code and datasets for classifying hotel reviews based on sentiment and ratings. The project leverages machine learning techniques to analyze customer reviews and predict sentiments (positive, neutral, negative) and ratings (1-5 stars). The goal is to provide insights into customer feedback for hotels.

---

## Repository Structure

```
hotel_review/
├── original_dataset/           # Contains the raw dataset files (to be downloaded from dataset source)
├── processed_dataset/          # Contains preprocessed datasets (generated using the original datsets downloaded by running code block in ipynb file)
├── rating_classification/      # Rating classification models and scripts 
├── sentiment_classification/   # Sentiment classification models and scripts
└── hotel_reviews_classification.ipynb  # Main Jupyter notebook for analysis
```

---

## Dataset

### Source
The dataset is sourced from [CMU Hotel Review Dataset](https://www.cs.cmu.edu/~jiweil/html/hotel-review.html). It consists of **878,561 reviews** (1.3GB) from **4,333 hotels**, crawled from TripAdvisor. Some reviews are in French.

### Files
- `review.txt`: Raw customer reviews.
- `offering.txt`: Metadata about hotels.

### Preprocessing
The raw dataset undergoes preprocessing to:
1. Remove non-English reviews using language detection.
2. Save cleaned English reviews to `processed_dataset/reviews_english.txt`.
3. Flatten metadata into structured CSV files (`offering.csv` and `reviews_english.csv`).

---

## Features

### Sentiment Classification
- Classifies reviews into **positive**, **neutral**, or **negative** sentiments.
- Metrics: Accuracy, Precision, Recall, F1-score.

### Rating Classification
- Predicts ratings on a scale of 1 to 5 stars.
- Metrics: Accuracy, Precision, Recall, F1-score.

---

## Usage

### Step 1: Download Dataset
Download the raw dataset files (`review.txt`, `offering.txt`) from [CMU Hotel Review Dataset](https://www.cs.cmu.edu/~jiweil/html/hotel-review.html) and place them in the `original_dataset/` folder.

### Step 2: Run Preprocessing
Execute the preprocessing cells in `hotel_reviews_classification.ipynb` to clean and structure the data.

### Step 3: Train Models
Use the notebook to train sentiment and rating classification models. The notebook includes:
- Data exploration.
- Model training and evaluation.
- Results visualization.

---

## Results

### Sentiment Classification Metrics
| Metric               | Value   |
|----------------------|---------|
| Accuracy             | 88.6%   |
| Macro Precision      | 79.8%   |
| Macro Recall         | 77.7%   |
| Weighted F1          | 88.3%   |

![Confusion Matrix](path/to/confusion_matrix_image.png)

### Rating Classification Metrics 
| Metric               | Value   |
|----------------------|---------|
| Accuracy             | 68.0%   |
| Macro Precision      | 64.5%   |
| Macro Recall         | 62.8%   |
| Weighted F1          | 67.8%   |

![Confusion Matrix](path/to/confusion_matrix_image.png)

---
