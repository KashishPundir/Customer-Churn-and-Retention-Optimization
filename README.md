# 📊 CUSTOMER CHURN, RETENTION & UPLIFT MODELING

---

## 🚀 OVERVIEW
This project focuses on analyzing customer behavior to **predict churn, explain model decisions, and move toward data-driven business actions**.

It combines:
- Machine Learning (Churn Prediction)
- Explainable AI (SHAP)
- Statistical Testing (T-Test)
- Feature Engineering
- Experimentation Thinking
- Uplift Modeling Concepts
- ROI-Based Decision Making

> ⚡ **Key Idea:** Prediction alone is not enough — real value comes from *profitable decision-making*.

---

## 🎯 OBJECTIVES
- Identify key drivers of customer churn  
- Build predictive models for churn probability  
- Transform raw data using feature engineering  
- Interpret predictions using SHAP  
- Validate results statistically  
- Introduce real-world ML concepts (uplift, ROI, experimentation)

---

## 📁 DATASET DESCRIPTION
The dataset includes customer transactional and behavioral features:

- `TotalOrder` → number of orders placed  
- `TotalItems` → total items purchased  
- `UniqueProducts` → product diversity  
- `TotalSpent` → total spending  
- `AvgOrderValue` → average value per order  
- `LastOrderValue` → most recent purchase value  
- Additional categorical features (country, item type, etc.)

> 📌 These features capture **customer engagement, value, and behavior patterns**.

---

## 🧱 FEATURE ENGINEERING (IMPORTANT)

Raw data was transformed into **more meaningful and informative features**.

### 🔄 WHAT WAS DONE:
- Created behavioral ratios (e.g., spending per order)
- Built engagement metrics (frequency, diversity)
- Aggregated features (totals vs averages)
- Applied scaling/normalization

### 💡 WHY IT MATTERS:
- Improves model performance  
- Reduces noise  
- Captures hidden behavioral signals  
- Enables better interpretation  

> ⚠️ **Without feature engineering, most ML models remain weak. This is a core strength of the project.**

---

## ⚙️ PROJECT WORKFLOW

### 1️⃣ DATA PREPROCESSING
- Handle missing values  
- Encode categorical variables  
- Normalize/scale features  

---

### 2️⃣ EXPLORATORY DATA ANALYSIS (EDA)
- Distribution analysis  
- Correlation study  
- Customer behavior patterns  

---

### 3️⃣ MODEL BUILDING
- Multiple ML models trained  
- Evaluated using:
  - AUC (Area Under Curve)
  - Log Loss
  - RMSE / MSE  

---

### 4️⃣ MODEL EXPLAINABILITY (SHAP)

SHAP explains predictions as:

Prediction = Base Value + Σ (Feature Contributions)

### 🔍 KEY INSIGHT:
- ~76% of prediction driven by **TotalOrder**
- Other features have much smaller impact  

> ⚠️ **Model is heavily dependent on a single feature → potential imbalance**

---

## 📊 STATISTICAL TESTING (T-TEST)

Example result:

```
t = -3.336
p = 0.000883
df = 890
```


### INTERPRETATION:
- p < 0.05 → statistically significant difference  
- Negative t → Group 1 mean < Group 2  

> ⚠️ **Important:** Statistical significance ≠ business importance

---

## 🔬 EXPERIMENTATION MINDSET

Prediction alone does not create value.

### REAL-WORLD APPROACH:
- Control Group → no action  
- Treatment Group → intervention (offer, call, etc.)  
- Compare results  

> 📌 This moves from **correlation → causation**

---

## 📈 UPLIFT MODELING (ADVANCED CONCEPT)

Traditional model:
> Who will churn?

Uplift model:
> Who will stay *because of our action*?

### CUSTOMER TYPES:
- Persuadables → target these ✅  
- Sure Things → waste ❌  
- Lost Causes → no impact ❌  
- Do Not Disturb → harmful ❌  

> 🎯 Only a small subset of customers actually create value

---

## 📊 QINI CURVE

Used to evaluate uplift models.

- Steeper curve → better targeting  
- Flat curve → random targeting  

> 📌 Replaces AUC in decision-focused systems

---

## 💰 ROI-BASED DECISION MAKING

Accuracy alone is not enough.

### FORMULA:
ROI = (Incremental Gain - Cost) / Cost

### INSIGHT:
- Wrong targeting = loss  
- Correct targeting = profit  

> ⚠️ A high-accuracy model can still lose money.

---

## 📉 KEY FINDINGS

### 1. DOMINANT FEATURE
- `TotalOrder` contributes ~76% of prediction  

### 2. BEHAVIORAL INSIGHT
- Low engagement strongly increases churn risk  

### 3. MODEL LIMITATION
- Weak contribution from other features  
- Possible over-reliance on one variable  

### 4. BUSINESS GAP
- Model predicts churn  
- Does NOT optimize intervention decisions  

---

## 🛠️ TECH STACK
- Python  
- Pandas, NumPy  
- Scikit-learn  
- SHAP  
- Matplotlib, Seaborn  

---

## 🎮 HOW TO USE THIS PROJECT

### BEGINNER
- Learn churn prediction  
- Understand SHAP  

### INTERMEDIATE
- Explore statistical testing  
- Analyze features  

### ADVANCED
- Extend into:
  - Uplift modeling  
  - Qini curve  
  - ROI optimization  

> 🚀 This is where real industry-level learning happens

---

## 📎 HOW TO RUN:

```bash
# Clone repository
git clone https://github.com/KashishPundir/Customer-Churn-and-Retention-Optimization.git

# Run notebook
jupyter notebook
```

## 🚀 CONCLUSION:

> A model that predicts churn but ignores ROI can destroy value.

This project highlights a critical shift:
- From accuracy → to impact  
- From prediction → to intervention  
- From modeling → to business strategy  

👉 The real power of data science is not prediction — it is **profitable action**.
