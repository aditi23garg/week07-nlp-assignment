# Week 07 — NLP Foundations Assignment

## 📌 Overview

This assignment focuses on handling complex NLP patterns in Indian e-commerce reviews and building an understanding of aspect-level sentiment classification.

The implementation covers:

* Negation handling
* Sarcasm detection
* Code-mixed text normalization
* Implicit sentiment detection
* Comparative sentence handling
* Aspect-level sentiment extraction

---

## 📂 Folder Structure

```
week07/
 ├── wednesday/
 │   ├── assignment.ipynb
 │   └── README.md
```

---

## ⚙️ Requirements

Install the required libraries before running the notebook:

```
pip install pandas numpy scikit-learn
```

---

## ▶️ How to Run

1. Clone the repository:

```
git clone <your-repo-link>
cd week07/monday
```

2. Open Jupyter Notebook:

```
jupyter notebook assignment.ipynb
```

3. Run all cells sequentially.

---

## 🧠 Key Concepts Implemented

### 1. Negation Handling

Transforms phrases like *“not bad”* into *“NOT_bad”* to correctly capture sentiment.

### 2. Sarcasm Detection

Identifies contrast between positive and negative expressions in the same sentence.

### 3. Code-Mixed Text Processing

Normalizes Hindi-English mixed text using dictionary-based mapping.

### 4. Implicit Sentiment Detection

Captures sentiment from actions (e.g., *“returned” → negative*).

### 5. Comparative Sentences

Extracts sentiment from comparisons like *“better than”*.

---

## 📊 Aspect-Level Sentiment Analysis

Extracts sentiment for individual aspects from a single review.

### Example:

**Input:**
“Amazing camera quality but the battery is atrocious and customer support was unhelpful.”

**Output:**

* Camera → Positive
* Battery → Negative
* Customer Support → Negative

---

## ⚠️ Limitations

* Rule-based methods may fail for unseen patterns
* Limited contextual understanding
* Performance depends on keyword matching

---

## 🚀 Future Improvements

* Use transformer-based models (e.g., BERT)
* Improve preprocessing and normalization
* Implement multi-label classification
* Use larger and more diverse datasets
