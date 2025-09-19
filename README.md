# Adult Income Classification - Machine Learning Project

## 📌 Overview
This project applies machine learning techniques on the **UCI Adult Census Income dataset** to predict whether an individual earns **more than $50K per year**.  
Developed during the **NTI Internship** as part of the Machine Learning track.

The project demonstrates:
- Data preprocessing and feature engineering
- Handling imbalanced datasets
- Applying supervised and unsupervised ML algorithms
- Model evaluation using metrics like accuracy, precision, recall, F1-score, and ROC-AUC
- Ensemble methods (Bagging, Boosting)
- Introduction to neural networks & deep learning

---

## 📊 Dataset
- **Source:** [UCI Adult Census Income Dataset (Kaggle)](https://www.kaggle.com/datasets/uciml/adult-census-income)  
- **Features:** Demographic and employment attributes (age, education, occupation, hours/week, etc.)  
- **Target:** `income` (<=50K or >50K)

> **Note:** Do *not* upload the raw dataset file to this repository. See *Download dataset* in Installation for instructions.

---

## ⚙️ Project Workflow
1. **Data Preprocessing**
   - Handling missing values & duplicates  
   - Encoding categorical variables  
   - Feature scaling  
   - Outlier detection & handling  
   - (Optionally) Balancing with SMOTE / class-weight strategies

2. **Feature Engineering**
   - Transformations (e.g. `log1p` for skewed features)  
   - Creating indicator features (e.g. `has_gain`)  
   - Feature selection using Mutual Information and model-based importances

3. **Models Applied**
   - Logistic Regression, KNN, SVM, Decision Tree, Random Forest, Naïve Bayes, XGBoost, Neural Networks

4. **Unsupervised Learning**
   - K-Means, DBSCAN, Gaussian Mixture Model, PCA

5. **Ensemble Methods**
   - Bagging (Random Forest), Boosting (XGBoost, AdaBoost)

6. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC, PR-AUC  
   - Visualizations: Confusion matrices, ROC/PR curves, feature importance

---

## 📈 Results (summary)
- Best performing model: **XGBoost** (AUC ≈ 0.92) after tuning and handling imbalance.  
- Random Forest and Decision Tree performed strongly as well.  
- Bernoulli Naïve Bayes served as a fast baseline because of many binary OHE features.

---
## install dependencies

pip install -r requirements.txt

---
## Download dataset (recommended approach)

Option A — manual download

Go to the Kaggle dataset page and download the adult.csv (or adult.data) file.

Put the file in the repository folder data/ (you may need to create the folder).

---
Option B — using Kaggle CLI (recommended for reproducibility)

# install kaggle CLI if needed
pip install kaggle
# configure (you need Kaggle API token in ~/.kaggle/kaggle.json)
kaggle datasets download -d uciml/adult-census-income -p data --unzip

---

## Run Jupyter Notebook

jupyter notebook

---
