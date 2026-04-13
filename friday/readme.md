# 📘 Week 07 — Friday Assignment

## 🧠 Assignment Overview

This assignment focuses on evaluating and selecting a sentiment classification model for the **ShopSense Reviews dataset**.

The goal is to:

* Understand why accuracy alone is misleading
* Evaluate models using proper metrics (Precision, Recall, F1-score)
* Compare models under real-world constraints
* Define a business cost model for prediction errors
* Recommend a production-ready solution with monitoring strategy

---

## 📂 Dataset

* **File:** `shopsense_reviews.csv`
* Contains:

  * Review text (`review_text`)
  * Sentiment labels (`sentiment_label`)
  * Language information (`language`)

---

## ⚙️ Folder Structure

```
week-07/
└── friday/
    ├── Assignment.ipynb
    └── README.md
```

---

## 🚀 How to Run

### 1️⃣ Clone Repository

```bash
git clone [<your-repo-link>](https://github.com/aditi23garg/week07
cd week-07/friday
```

### 2️⃣ Install Requirements

```bash
pip install pandas numpy scikit-learn
```

### 3️⃣ Run Notebook

* Open Jupyter Notebook / VS Code
* Run all cells in order:

  * Preconditions (data loading, preprocessing, model training)
  * Sub-step 1 → 5

---

## 🔍 Key Steps Covered

### 🟢 Easy

* Class distribution analysis
* Model evaluation using F1-score, Precision, Recall

### 🟡 Medium

* Model comparison (Logistic Regression vs Naive Bayes)
* Latency and Hinglish evaluation
* Cost model (FN vs FP impact)
* Production recommendation + monitoring plan

---

## 💼 Business Insight

* Accuracy alone is misleading due to class imbalance
* Missing negative reviews (complaints) has higher business cost
* Logistic Regression chosen due to:

  * Lower misclassification cost
  * Strong performance
  * Fast inference

---

## 📊 Final Recommendation

* Deploy **Logistic Regression (TF-IDF)**
* Track **Recall (Negative class)** weekly
* Retrain if performance drops below threshold

---

## ⚠️ Notes

* No hardcoded file paths used
* Modular code with functions
* All steps executed sequentially

---

## 🛠️ Tech Stack

* Python 3.x
* Pandas
* NumPy
* Scikit-learn

