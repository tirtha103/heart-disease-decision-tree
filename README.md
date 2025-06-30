#  Heart Disease Prediction using Decision Trees & Random Forests

>  Tree-Based Machine Learning Models  
>  Completed by: Tirtha Dutta  
>  Project Type: Classification | 📊 Model Type: Supervised Learning  

---

##  Objective

Build and evaluate machine learning models (**Decision Tree** and **Random Forest**) to predict the presence of heart disease from patient health records. This is an internship submission that demonstrates the full data science workflow — from cleaning to model evaluation.

---

##  Dataset

- **Source:** [Heart Disease Dataset – Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)  
- **Shape (after cleaning):** `302 rows × 14 columns`  
- **Target Column:** `target` (`0 = No Heart Disease`, `1 = Heart Disease`)

---

##  Workflow Summary

### 1️ Data Cleaning & Preprocessing
- Removed **723 duplicate rows**
- Verified **no missing/null values**
- Verified and fixed data types for modeling

### 2️ Exploratory Data Analysis (EDA)
- Visualized **outliers** with boxplots
- Generated **heatmap** for correlation analysis

### 3️ Model Building
- Trained a **Decision Tree Classifier**  
  - Accuracy: `73.77%`
- Applied **pruning** (`max_depth=4`)  
  - Accuracy remained: `73.77%`
- Trained a **Random Forest Classifier**  
  - Accuracy: **`83.61%`**  Best
- Visualized decision paths and **feature importances**

### 4️ Evaluation
- Compared model performance
- Used accuracy and visualization tools
- Performed **k-fold cross-validation** for reliability

---

##  Feature Importance (Top Predictors)

| Rank | Feature   | Description                              |
|------|-----------|------------------------------------------|
| 1️   | `thalach` | Max heart rate during exercise           |
| 2️   | `cp`      | Type of chest pain                       |
| 3️   | `oldpeak` | ST depression on ECG after stress        |

These were identified by Random Forest as most critical in predicting heart disease.

---

##  Results

| Model Type            | Accuracy (%) |
|-----------------------|--------------|
| Decision Tree         | 73.77%       |
| Pruned Decision Tree  | 73.77%       |
|  Random Forest (Best) | **83.61%**   |

---


---

##  Tools & Libraries

See `requirements.txt` for installation, or run:

```bash
pip install -r requirements.txt


