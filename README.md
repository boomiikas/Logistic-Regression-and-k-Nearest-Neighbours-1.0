# 📊 Machine Learning Experiments

This repository explores **Classification and Regression** tasks using multiple datasets.  
We apply models such as **Logistic Regression** and **K-Nearest Neighbors (KNN) Regression**, and evaluate them using standard ML metrics.

---

## 📂 Datasets

### 1. 🏠 Airbnb Dataset (`airbnb.csv`)
**Columns:**
- `size_m2` → Size of the property in square meters  
- `distance_center_km` → Distance from city center  
- `rating` → Average rating given by guests  
- `num_reviews` → Number of reviews  
- `price` → Target variable (Property price in $)  

**Task:** Regression → Predict property price using features.

---

### 2. 🌸 Flower Dataset (`flower.csv`)
**Columns:**
- `sepal_length`  
- `sepal_width`  
- `petal_length`  
- `petal_width`  
- `species` → Target variable (Flower type)  

**Task:** Classification → Identify flower species (Iris dataset style).

---

### 3. 🧬 Disease Stage Dataset (`disease_stage.csv`)
**Columns:**
- `age`  
- `b1`, `b2`, `b3`, `b4` → Biomarker levels  
- `stage` → Target variable (Disease stage: 0/1)  

**Task:** Classification → Predict disease stage using Logistic Regression.

---

### 4. 👩‍💻 Customer Churn Dataset (`customer_churn.csv`)
**Columns:**
- `tenure_months`  
- `monthly_charges`  
- `support_tickets`  
- `is_premium` (0 = no, 1 = yes)  
- `avg_usage_hours`  
- `churn` → Target variable (1 = customer churned, 0 = retained)  

**Task:** Classification → Predict customer churn likelihood.

---

### 5. 📧 Email Spam Dataset (`email_spam.csv`)
**Columns:**
- `word_free`  
- `word_offer`  
- `word_click`  
- `num_links`  
- `num_caps` → Number of capital letters  
- `sender_reputation`  
- `is_spam` → Target variable (1 = spam, 0 = not spam)  

**Task:** Classification → Detect spam emails.

---

## ⚙️ Workflow

1. **Data Preprocessing**
   - Handle missing values  
   - Encode categorical columns (if any)  
   - Scale features using **StandardScaler**  

2. **Train-Test Split**
   - 80% training, 20% testing  

3. **Model Training**
   - Logistic Regression → For classification tasks  
   - KNN Regression → For regression tasks (Airbnb dataset)  
   - GridSearchCV → For hyperparameter tuning (`n_neighbors`)  

4. **Evaluation**
   - **Classification Metrics:**
     - Accuracy  
     - Precision  
     - Recall  
     - F1-Score  
     - ROC-AUC  
     - Confusion Matrix  

   - **Regression Metrics:**
     - RMSE (Root Mean Squared Error)  
     - R² Score (Coefficient of Determination)  

---
