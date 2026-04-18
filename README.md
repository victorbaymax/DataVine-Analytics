# 🛒 Customer & Product Analytics with PCA, k-NN, and Clustering

This project explores customer and product behavior using a mix of dimensionality reduction, classification, recommendation systems, and clustering techniques. In other words: turning messy retail data into something actually useful (and slightly less painful to look at).

---

## 📦 Dataset

The analysis is based on two prepared datasets:

* `customer_level_online_retail.csv`
* `product_level_online_retail.csv`

These datasets contain aggregated information about:

* Customer purchasing behavior
* Product performance and engagement

---

## 🔧 What This Project Covers

### 1. Data Preparation

* Loaded and inspected datasets
* Checked for missing values and inconsistencies
* Standardized numerical features for modeling

---

### 2. Customer Classification (k-NN + PCA)

* Applied **PCA** to retain 95% variance
* Tuned hyperparameters using **GridSearchCV**
* Trained a **k-Nearest Neighbors classifier**
* Evaluated performance with:

  * Accuracy score
  * Classification report
  * Confusion matrix

💡 *Goal:* Predict customer segments without accidentally cheating (no data leakage allowed).

---

### 3. Product Recommendation System

* Reduced product features using **PCA (1 component)**
* Used **cosine similarity** via Nearest Neighbors
* Built a simple recommendation engine:

  * Input: one product
  * Output: similar products

💡 *Goal:* “If you liked this, you might also like…” but without needing a billion-dollar ML team.

---

### 4. Crime Clustering (USArrests-style Analysis)

*(Adapted to dataset context)*

* Standardized features
* Selected top variables
* Applied **PCA (2 components)**
* Compared clustering methods:

  * **K-Means** (hard clustering)
  * **GMM** (probabilistic clustering)
* Evaluated:

  * Elbow method (K-Means)
  * BIC (GMM)

💡 *Goal:* Group data points and argue about which clustering method is “better” like true data scientists.

---

## 🧠 Key Concepts Used

* Principal Component Analysis (PCA)
* k-Nearest Neighbors (k-NN)
* GridSearchCV (hyperparameter tuning)
* Cosine Similarity
* K-Means Clustering
* Gaussian Mixture Models (GMM)
* Feature Scaling (Standardization)

---

## 📊 Key Takeaways

* PCA helps reduce noise and improve model performance across multiple tasks
* Removing leakage-prone variables is critical for realistic model evaluation
* k-NN works well with proper tuning and dimensionality reduction
* GMM provides more flexible clustering than K-Means
* Product similarity models are immediately actionable for business use

---

## 🚀 How to Run

1. Clone the repo:

```bash
git clone https://github.com/yourusername/your-repo-name.git
```

2. Open the notebook:

```bash
jupyter notebook C08_M08_completed.ipynb
```

3. Run all cells and enjoy watching your laptop do math.

---

## ⚠️ Notes

* Make sure required libraries are installed:

  * `pandas`
  * `numpy`
  * `scikit-learn`
  * `matplotlib`
  * `seaborn`

* If something breaks… it’s probably a missing import or a typo (we’ve all been there).

---

## 😂 Final Thought

This project proves two things:

1. Data can be turned into insights
2. And bugs can be turned into character development

---

If you want, I can also tailor this README with your GitHub username, repo name, or make it more “recruiter-friendly” (slightly less jokes, slightly more buzzwords).
