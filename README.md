# Bank Account Fraud — KMeans, LazyPredict, KNN, MLP

This repo explores the **NeurIPS 2022 Bank Account Fraud** dataset with:
- **Unsupervised:** K-Means clustering
- **Model selection:** LazyPredict to scan many classifiers quickly
- **Supervised:** **KNN** and **MLP** (with cross-validation)

It follows the course assignment in `HW5_Guide.pdf` and the final write-up in `project5report.pdf` (Persian). 

---

## Dataset

Kaggle: https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022  
**Use `base.csv`** for best results 


---

## What’s here

- `model.ipynb` — main notebook: preprocessing → KMeans → LazyPredict scan → KNN/MLP + CV → metrics/plots  
- `HW5_Guide.pdf` — assignment brief (datasets to choose from, steps, and marking). 
- `project5report.pdf` — final report (Persian) with method details, figures, and observations. 

---

## Quick start

1. Download **`base.csv`** from the Kaggle page and put it **outside** Git (e.g., `data/base.csv`).
2. Open `model.ipynb` in Jupyter and run top-to-bottom.  
3. If the notebook expects a different path, change the read path at the top (e.g., `pd.read_csv("data/base.csv")`).

**Dependencies:** this is a standard PyData stack — `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, plus `lazypredict`. Install on the fly if needed:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn lazypredict
