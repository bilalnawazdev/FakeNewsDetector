# 📰 Fake News Detection using BERT & TF-IDF

This project is focused on detecting fake news articles using Natural Language Processing (NLP) techniques. I experimented with both traditional ML (TF-IDF + Random Forest) and a transformer-based deep learning model (BERT) to classify news articles as real or fake.

---

## 📊 Dataset

The dataset used is a publicly available Kaggle dataset with over **50,000 news articles** labeled as either real or fake.

---

## 🔍 Models Implemented

### 1. TF-IDF + Random Forest (Baseline)
- Preprocessing: lowercasing, punctuation removal, stopwords.
- Feature extraction: TF-IDF Vectorizer
- Model: RandomForestClassifier
- Accuracy: ~84%

### 2. BERT (Transformer-based)
- Tokenization: `BertTokenizer` from HuggingFace
- Model: `BertForSequenceClassification`
- Training: Fine-tuned on 80/20 train-test split
- Accuracy: **92%**

---

## 🌐 Deployment

The final BERT model is deployed using a **Flask API**. You can send a POST request with a news article, and it returns whether it's "FAKE" or "REAL".

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- scikit-learn
- Transformers (HuggingFace)
- PyTorch
- Flask
- Matplotlib, Seaborn

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/bilalnawazdev/FakeNewsDetector.git

2. Install Dependencies
```bash
pip install -r requirements.txt

3. Run the Flask App
```bash
cd app
python app.py

