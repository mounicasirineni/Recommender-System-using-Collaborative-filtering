# Recommender System using Collaborative Filtering

> **📚 Course Project** | IDS 572: Data Mining for Business  
> **🏫 University of Illinois at Chicago**  
> **⏰ Completed:** Fall 2015  
> **📝 Last Updated:** February 2026 (documentation only)  
> **🔍 [View Development Timeline](../../commits/main)** - See original commits from Fall 2015

---

## Overview

Built a movie recommendation engine using collaborative filtering techniques on the MovieLens dataset as part of the Data Mining for Business course. Implemented both user-based and item-based approaches, as well as matrix factorization using SVD, to predict user ratings and generate personalized movie recommendations.

**Course:** IDS 572 - Data Mining for Business  
**Technologies:** Python, Scikit-learn, Pandas, NumPy, Matplotlib

---

## Technical Approach

### 1. Data Processing
- Loaded MovieLens dataset with 100k+ movie ratings
- Created user-item rating matrix
- Handled sparse data (99%+ sparsity)
- Split data into training and test sets (80/20)

### 2. Algorithms Implemented

**User-Based Collaborative Filtering:**
- Calculated user similarity using Pearson correlation coefficient
- Identified k-nearest neighbors for each user
- Generated predictions based on weighted average of similar users' ratings

**Item-Based Collaborative Filtering:**
- Computed item similarity using cosine similarity
- Found similar movies for each item
- Made predictions based on user's ratings of similar items

**Matrix Factorization (SVD):**
- Implemented Singular Value Decomposition
- Optimized latent factors to capture user preferences and item characteristics
- Tuned hyperparameters (number of factors, learning rate)

### 3. Evaluation Metrics
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Compared performance across different algorithms

---

## Results

- **Item-based CF** outperformed user-based approach with lower RMSE
- **Matrix factorization (SVD)** achieved best overall accuracy (RMSE < 0.9)
- Successfully handled highly sparse user-item matrices
- Identified trade-offs between accuracy and computational efficiency

---

## Key Learnings

1. **Sparse Data Handling:** Learned techniques to work with highly sparse matrices common in real-world recommendation systems
2. **Similarity Metrics:** Understanding when to use Pearson correlation vs. cosine similarity based on data characteristics
3. **Scalability:** Item-based collaborative filtering scales better than user-based for large user bases
4. **Matrix Factorization:** SVD effectively reduces dimensionality while capturing latent user-item relationships
5. **Cold Start Problem:** Recognized challenges in recommending for new users/items with limited interaction history

---

## Skills Demonstrated

- Recommendation Systems
- Collaborative Filtering
- Matrix Factorization
- Machine Learning
- Python Programming
- Data Preprocessing
- Model Evaluation

---

## Academic Context

This project was part of **IDS 572: Data Mining for Business** at UIC, completed in **Fall 2015**—years before recommendation systems became ubiquitous in modern platforms. The techniques learned here (similarity metrics, matrix factorization, handling sparse data) remain fundamental to recommendation engines at companies like Netflix, Amazon, and Spotify.

---

**[← Back to Portfolio](https://github.com/mounicasirineni/masters-ml-portfolio)**
