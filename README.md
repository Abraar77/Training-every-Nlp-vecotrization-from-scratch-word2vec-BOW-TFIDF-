# NLP Text Classification using Word2Vec and AvgWord2Vec

This repository demonstrates an end-to-end **NLP text classification pipeline** using  
**Word2Vec** and **Average Word2Vec (AvgWord2Vec)** for feature extraction, followed by a  
**RandomForest Classifier** with **GridSearchCV** for hyperparameter optimization.

---

## Project Overview

Traditional text data cannot be directly fed into machine learning models.  
In this project, raw text is transformed into numerical vectors using **Word2Vec embeddings**,  
and sentence-level representations are generated using **AvgWord2Vec**.

These vectors are then used to train a **RandomForest classifier**, with model performance improved by tuning hyperparameters using **GridSearchCV**.

---

## Workflow

1. **Text Preprocessing**
   - Lowercasing
   - Tokenization
   - Stopword removal
   - Text cleaning

2. **Word Embedding Generation**
   - Train a Word2Vec model on the corpus
   - Generate word-level embeddings

3. **AvgWord2Vec Feature Engineering**
   - Compute sentence vectors by averaging word embeddings
   - Convert each text sample into a fixed-length numeric vector

4. **Model Building**
   - Train a RandomForest Classifier
   - Use GridSearchCV to find optimal hyperparameters

5. **Evaluation**
   - Accuracy score
   - Model comparison after hyperparameter tuning

---

## Repository Structure

