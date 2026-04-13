# Week 07 — NLP Assignment (Word2Vec, Similarity, Semantic Gap)

## 📌 Overview

This assignment focuses on:

* Training Word2Vec on ShopSense reviews
* Understanding polysemy using the word "cheap"
* Performing word sense disambiguation using context
* Comparing sentence similarity using different techniques
* Understanding semantic gap in NLP models

---

## 📂 Dataset

* ShopSense E-Commerce Reviews dataset
* Contains review text, ratings, sentiment labels, etc.

---

## ⚙️ Installation

Install required libraries:

```bash
pip install pandas numpy gensim scikit-learn sentence-transformers
```

---

## ▶️ How to Run

1. Open Jupyter Notebook:

```bash
jupyter notebook
```

2. Navigate to:

```
week07/tuesday/assignment.ipynb
```

3. Run all cells sequentially

---

## 📊 Tasks Covered

### ✅ Q1(a): Word2Vec Polysemy

* Trained Word2Vec model
* Demonstrated that "cheap" has a single embedding
* Used cosine similarity with dataset-based similar words

### ✅ Q1(b): Word Sense Disambiguation

* Built a context-based classifier
* Used anchor vectors for:

  * Affordable meaning
  * Low-quality meaning
* Explained limitations due to rare/missing words

### ✅ Q1(c): Window Size Comparison

* Compared window size = 2 vs 10
* Observed syntactic vs semantic relationships

---

### ✅ Q2: Sentence Similarity

Compared similarity between two reviews using:

* Bag of Words (BOW)
* TF-IDF
* Word2Vec (averaging)
* Sentence-BERT

---

## 📈 Key Observations

* Word2Vec cannot handle polysemy directly (single vector per word)
* Missing/rare words affect embedding quality (OOV problem)
* BOW fails due to lack of word overlap
* Sentence-BERT performs best for semantic similarity

---

## 📌 Output

* Cosine similarity scores for all methods
* Word similarity results for "cheap"
* Disambiguation predictions
* Comparison of window sizes

---

## 🚀 Conclusion

* Context is essential for understanding word meaning
* Traditional methods fail to capture semantics
* Transformer-based models (SBERT) perform best

