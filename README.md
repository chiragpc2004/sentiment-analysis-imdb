# 🎬 IMDB Sentiment Analysis

This project builds a sentiment classification pipeline using the IMDB 50K Movie Reviews Dataset. We explore both traditional machine learning models and deep learning (LSTM) to classify reviews as **Positive** or **Negative**.


## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/chiragpc2004/sentiment-analysis-imdb.git
cd sentiment-analysis-imdb
```

2. Create a virtual environment and install dependencies:

```bash
python -m venv venv
source venv/bin/activate     # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

---

## 📊 Dataset

We use the [IMDB Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/data), which contains:

- 50,000 movie reviews
- Balanced: 25,000 positive and 25,000 negative
- Pre-split into 25k training and 25k testing samples

---

## 🧹 Preprocessing

Text data is cleaned and prepared through:

- Lowercasing
- Removing HTML tags, punctuation, and stopwords
- Tokenization
- Padding/truncating for deep learning models

---

## 🧠 Models Used

### ✅ **Machine Learning Models**
1. **Logistic Regression** – Interpretable and reliable baseline.
2. **Naive Bayes** – Works well for text classification.
3. **Gradient Boosting (XGBoost)** – Advanced ensemble model.

### 🧠 **Deep Learning Model**
- **LSTM (Long Short-Term Memory)** neural network:
  - Input: Sequences via `Tokenizer` and `pad_sequences`
  - Architecture: `Embedding` → `LSTM` → `Dense`
  - Trained with binary cross-entropy

---

## 📈 Evaluation

Model performance is assessed using:

- **Accuracy Score**
- **Confusion Matrix**
- **Loss Fucnction**

---

## ✅ Results

| Model               | Accuracy  |
|--------------------|------------|
| Logistic Regression| ~88%       |
| Naive Bayes        | ~86%       |
| Gradient Boosting  | ~84%       |
| **LSTM**           | **95-97%** |

---

## 👨‍💻 Author

Chirag Poojarikodi  
📧 chiragpc2004@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/chiragpc2004) | [GitHub](https://github.com/chiragpc2004)

---
