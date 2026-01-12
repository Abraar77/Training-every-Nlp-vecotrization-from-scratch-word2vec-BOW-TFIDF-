# NLP Vectorization Techniques — From Scratch

This project demonstrates the implementation of multiple **text vectorization techniques** from scratch and using standard Python libraries.  
It includes approaches such as **Bag of Words (BoW)**, **TF-IDF**, and **Word2Vec** — each transforming raw text into numerical vector representations suitable for machine learning. :contentReference[oaicite:0]{index=0}

---

## 📌 Overview

In Natural Language Processing (NLP), machine learning models cannot work directly with raw text data.  
Text vectorization transforms words and documents into numerical vectors that algorithms can process. :contentReference[oaicite:1]{index=1}

This project covers:

- **Bag of Words (BoW)**
- **Term Frequency-Inverse Document Frequency (TF-IDF)**
- **Training Word2Vec from scratch**

These techniques differ in how they represent text:

| Technique | Key Idea | Contextual Semantics |
|-----------|----------|---------------------|
| BoW | Count of words in text | ❌ |
| TF-IDF | Weighted word counts | ❌ (weights rare words more) |
| Word2Vec | Predictive word embeddings | ✔️ (captures semantic relationships) | :contentReference[oaicite:2]{index=2}

---

## 🧠 What You Will Learn

### 1. Bag of Words (BoW)

- Converts text into a matrix of token counts.
- Simple and effective for many baseline models.
- Does not capture word order or semantics. :contentReference[oaicite:3]{index=3}

### 2. TF-IDF

- Counts words while down-weighting common words.
- Improves over BoW for many NLP tasks.
- Still does not capture deep contextual meaning. :contentReference[oaicite:4]{index=4}

### 3. Word2Vec

- Trains dense vector representations for words.
- Represents semantics; words with similar meaning have vectors near each other. :contentReference[oaicite:5]{index=5}
- This repository includes a training pipeline using **Gensim’s Word2Vec implementation** (e.g., CBOW or Skip-Gram).

---

You will see how is wrod2vec best of them all, it word2vec accuracy went up tp 98% while in bow and tfidf it was barely 88%

## 📁 Project Structure

```

Training word2vec from scratch/
├── dataset/                       # Text datasets (if included)
     └──spamCollection.csv
├── notebooks/                             # Jupyter notebooks
│   └── finalmodel.ipynb            # Main demo for BoW, TF-IDF & Word2Vec
                            

````

---

## 🛠 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Abraar77/Training-every-Nlp-vecotrization-from-scratch-word2vec-BOW-TFIDF-.git
   cd Training-every-Nlp-vecotrization-from-scratch-word2vec-BOW-TFIDF-/Training\ word2vec\ from\ scratch
````

2. Create and activate a virtual environment (optional):

   ```bash
   python3 -m venv venv
   source venv/bin/activate      # macOS/Linux
   venv\Scripts\activate         # Windows
   ```

---

## 🧪 How to Use

1. Open the main vectorization notebook:

   ```bash
   jupyter notebook notebooks/NLP-vectorization.ipynb
   ```

2. Run through the cells to:

   * Clean and preprocess text
   * Train vectorizers (BoW, TF-IDF)
   * Train Word2Vec embeddings from scratch
   * Inspect vector representations and visualize similarities

---

## 🧾 Example Insight

Once trained, the **Word2Vec vectors** can be used to:

* Visualize semantic clusters of words
* Compute similarity between words
* Feed into downstream models for classification or clustering

---
