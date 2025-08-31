# 🎬 Recommender Systems with Python

This repository demonstrates how to build **Recommender Systems** using Python and the **MovieLens dataset**.  
It includes both a **basic content-based recommender** (using similarity of movies) and **advanced collaborative filtering techniques** (memory-based and model-based).  

The project serves as an introduction to recommendation engines and a stepping stone to more advanced techniques used in real-world applications (e.g., Netflix, Spotify, Amazon).

---

## 📁 Project Overview

### 🔹 Basic Recommender (Content-Based)
- Built using **Pandas**.
- Suggests movies that are most similar to a chosen movie based on user ratings.
- Simple introduction to recommendation systems (not a full production-ready system).

### 🔹 Advanced Recommenders
1. **Collaborative Filtering (CF)**
   - Uses the “wisdom of the crowd” to recommend items based on user-item interactions.
   - Two approaches implemented:
     - **Memory-Based CF**: Cosine similarity between users or items.
     - **Model-Based CF**: Singular Value Decomposition (SVD) for matrix factorization.
   - Allows feature learning from user-item rating matrices.

2. **Content-Based Recommender**
   - Focuses on movie attributes (metadata).
   - Recommends similar movies to the one selected by the user.

---

## 📊 Dataset

- **MovieLens 100k Dataset**  
  - 100,000 ratings from 943 users on 1,682 movies.  
  - Common benchmark dataset for recommender systems.  
- Format: `user_id | item_id | rating | timestamp`

📥 [Download MovieLens Dataset](https://grouplens.org/datasets/movielens/)  

---

## 🛠️ Tech Stack

- **Python**  
- **Pandas, NumPy** → Data manipulation  
- **Matplotlib, Seaborn** → Data visualization  
- **Scikit-learn** → Similarity metrics (cosine similarity, train/test split)  
- **SciPy** → Singular Value Decomposition (SVD)  

---

## 🔎 Steps Involved

1. **Data Exploration & Cleaning**  
   - Loaded MovieLens dataset.  
   - Processed user-item rating matrix.  

2. **Basic Recommender (Content-Based)**  
   - Recommend movies most similar to a given movie using correlations.  

3. **Collaborative Filtering**  
   - **Memory-Based**: Calculated similarity between users/items using cosine similarity.  
   - **Model-Based**: Applied matrix factorization with SVD for dimensionality reduction.  

4. **Evaluation**  
   - Compared predictions with actual ratings.  
   - Measured accuracy using RMSE (Root Mean Square Error).  

---

## 📈 Results & Insights

- **Content-Based Recommender**: Good for suggesting movies similar to the user’s choice but limited in personalization.  
- **Collaborative Filtering**: More powerful because it leverages crowd wisdom.  
- **SVD-based Model**: Provided better recommendations with reduced dimensionality and improved generalization.  

---

## 🚀 Future Work

- Implement **Hybrid Recommender Systems** (combining CF + content-based).  
- Try **Deep Learning-based recommenders** (e.g., Neural Collaborative Filtering).  
- Deploy using **Streamlit or Flask** for interactive movie recommendations.  

---
