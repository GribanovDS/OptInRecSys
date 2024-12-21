# Optimization Methods in Recommender Systems

## Project Overview
This project investigates **Recommender Systems (RecSys)** using **Matrix Factorization** as the primary approach for modeling user-item interactions. The goal is to minimize the **loss function** through optimization techniques and compare their performance in terms of predictive accuracy and ranking quality.

The project focuses on exploring and implementing various **optimization algorithms** to improve training efficiency and recommendation quality.

---

## Optimization Algorithms Used
The following optimization algorithms were implemented and evaluated:
1. **Stochastic Gradient Descent (SGD)**
2. **Momentum**
3. **Nesterov Momentum**
4. **RMSProp**
5. **Adam**
6. **AdamW**
7. **Adagrad**
8. **Nadam**
9. **AdaMax**
10. **Adadelta**

Grid search was used for **hyperparameter tuning**, and each algorithm was evaluated based on **RMSE**, **Precision@K**, **Recall@K**.

---

## Code Structure
All code is provided in a **Jupyter Notebook (.ipynb)** file for easy execution and reproducibility.  
- The notebook contains:
  - **Data Preprocessing**
  - **Baseline Models (Global Mean, User Mean, Item Mean)**
  - **Matrix Factorization Implementation**
  - **Evaluation Metrics Calculation**
  - **Hyperparameter Tuning via Grid Search**
  - **Comparison of Optimizers**

---

## Datasets

1. **[MovieLens Dataset](https://grouplens.org/datasets/movielens/)** (/data)  
   - Explicit ratings dataset with 100,000 ratings from 943 users on 1,682 movies.
   - Used for benchmarking optimizers with user-item interactions.

2. **[Last.fm Dataset](http://millionsongdataset.com/lastfm/)** (/lastfm)
   - Implicit feedback dataset containing listening counts for artists by users.
   - Includes 92,834 interactions between 1,892 users and 17,632 artists.

Both datasets are available at repository

---

## Results and Evaluation
Statistical improvements were observed over the baseline models (Global Mean) using advanced optimizers.  
Key metrics are summarized below:

| Model                        | RMSE   | Precision@10 | Recall@10 |
|------------------------------|--------|--------------|-----------|
| Global Mean Baseline         | 1.25   | 0.12         | 0.08      |
| Matrix Factorization (Adam)  | 0.75   | 0.27         | 0.22      |


