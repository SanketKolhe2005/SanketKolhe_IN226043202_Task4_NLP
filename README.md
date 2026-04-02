# 🚀 NLP Task 4: Fine-Tuning BERT on IMDB Dataset

## 📌 Project Overview

This project focuses on fine-tuning a pre-trained **BERT (Bidirectional Encoder Representations from Transformers)** model for sentiment classification using the IMDB Movie Reviews dataset. The goal is to classify reviews as **positive** or **negative**.

---

## 🎯 Objective

* Understand BERT architecture for text classification

* Perform fine-tuning using Hugging Face Transformers

* Apply tokenization using pre-trained models

* Evaluate model using classification metrics

* Perform experiments and compare results

---

## 🛠️ Technologies Used

* Python

* PyTorch

* Hugging Face Transformers

* Scikit-learn

* Jupyter Notebook / Google Colab

---

## 📂 Dataset

* **Dataset Used:** IMDB Movie Reviews Dataset

* **Source:** Kaggle

* **Size:** 50,000 reviews

---

## ⚙️ Project Pipeline

```
Raw Data → Preprocessing → Tokenization → Model Training → Evaluation → Comparison
```

---

## 🔹 Steps Performed

### 1. Data Preprocessing

* Removed missing values

* Converted labels (positive → 1, negative → 0)

* Renamed columns for consistency

### 2. Data Splitting

* Training Set: 70%

* Validation Set: 15%

* Test Set: 15%

### 3. Tokenization

* Used `bert-base-uncased` tokenizer

* Converted text into token IDs

### 4. Model Building

* Used `AutoModelForSequenceClassification`

* Pre-trained BERT model

### 5. Fine-Tuning

* Optimizer: AdamW

* Learning Rate: 2e-5

* Epochs: 2

---

## 📊 Model Evaluation

The model was evaluated using:

* Accuracy

* Precision

* Recall

* F1 Score

* Confusion Matrix

---

## 🔬 Experiments

### ✅ Experiment 1: Freeze BERT Layers

* Faster training

* Lower accuracy

### ✅ Experiment 2: Fine-Tune Last 2 Layers

* Balanced performance

* Improved accuracy

### ✅ Full Fine-Tuning

* Highest accuracy
  
* More training time

---

## 📈 Results & Analysis

* Full fine-tuning produced the best performance
  
* Freezing layers reduced computation but affected accuracy
  
* Partial fine-tuning provided a good balance

---

## ⚠️ Note

Due to a known issue with `Trainer.evaluate()` in some environments, evaluation was performed using the `predict()` method along with sklearn metrics.

---

## 🚀 Future Improvements

* Try DistilBERT or RoBERTa
  
* Use learning rate scheduler
  
* Implement early stopping
  
* Hyperparameter tuning

---
## 🚀 Open in Colab

https://colab.research.google.com/github/SanketKolhe2005/SanketKolhe_IN226043202_Task-4_NLP/blob/main/Task4_NLP.ipynb

---

## 📌 Conclusion

BERT is highly effective for sentiment classification tasks. Fine-tuning significantly improves performance compared to traditional machine learning approaches.
