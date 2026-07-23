# Category Identification in Data via Machine Learning

Automated product categorization and feature-based recommendation system designed for e-commerce platforms using supervised machine learning and vector similarity algorithms.

## Overview
As e-commerce catalogs grow rapidly, manual classification and fixed rule-based systems struggle to maintain speed and accuracy. Misclassified products directly lead to poor search performance and reduced user engagement. 

This project addresses these issues through a dual-approach architecture:
1. **Supervised Classification:** Uses a **Random Forest Classifier** to assign unseen products to correct categories based on numeric attributes (e.g., price, discount, ratings).
2. **Content-Based Recommendation:** Employs **Cosine Similarity** to compute distance vectors between items to recommend highly similar products in real time.

## Key Features
* **Automated Product Tagging:** Replaces error-prone manual labeling with high-accuracy machine learning predictions.
* **Content-Based Filtering:** Recommends items based on shared feature traits rather than overall popularity.
* **Benchmark Comparison:** Evaluated against **K-Means Clustering** to show the advantages of supervised ensemble methods over unsupervised grouping.

## Tech Stack & Dependencies
* **Language:** Python 3.x
* **Core Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`
* **Development Environment:** Jupyter Notebook / VS Code / Spyder

## Architecture & Workflow
1. **Data Preprocessing:** Standard scaling, label encoding, handling missing values, and dropping low-frequency categories.
2. **Data Division:** Train-test split (80:20 ratio).
3. **Model Training:** Random Forest Classifier trained on preprocessed feature vectors.
4. **Similarity Engine:** Multi-dimensional Cosine Similarity calculated across normalized numerical features.

## Results & Performance Metrics
* **Random Forest Accuracy:** **84.82%**
* **K-Means Clustering Accuracy:** **69.11%**

### Quantitative Classification Summary (Random Forest)
| Category | Precision | Recall | F1-Score | Support |
| :--- | :--- | :--- | :--- | :--- |
| **Cameras** | 0.91 | 0.91 | 0.91 | 86 |
| **Laptops** | 0.82 | 0.86 | 0.84 | 85 |
| **Phones** | 0.87 | 0.94 | 0.90 | 105 |
| **Smart Home** | 0.94 | 0.71 | 0.81 | 24 |
| **Printers & Scanners** | 0.91 | 0.05 | 0.09 | 21 |
| **Weighted Average** | **0.85** | **0.85** | **0.84** | **369** |

---
*Developed as part of the B.E. in Electronics and Communication Engineering at New Horizon College of Engineering (VTU).*
