# Web link

https://spamorham-classifier.streamlit.app/

# 📱 SMS Spam Classifier

A simple and interactive web application built with **Streamlit** that classifies SMS messages as **Spam** or **Ham (Not Spam)** using a trained machine learning model.

---

## 🚀 Features

- ✅ Paste any SMS message and instantly receive a classification
- 📊 Displays confidence score along with the prediction
- 💡 Clean and user-friendly interface
- 🧠 Uses a trained model and TF-IDF vectorizer from `scikit-learn`

---

## 🧠 How It Works

The app loads a pre-trained machine learning model (`spam_classifier.pkl`) and a corresponding text vectorizer (`vectorizer.pkl`). When a message is entered, it is vectorized and passed to the model to predict:

- **SPAM**: Unwanted or junk message
- **HAM**: Legitimate message

---

## 🧪 Model & Vectorizer

- **Model**: Any `scikit-learn`-compatible classifier (e.g., Naive Bayes, Logistic Regression)
- **Vectorizer**: TF-IDF vectorizer trained on the SMS dataset (e.g., [UCI SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset))

---

## 🖥 How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/sms-spam-classifier.git
cd sms-spam-classifier
python -m venv .venv
.\.venv\Scripts\activate    # Windows
# or: source .venv/bin/activate  # macOS/Linux
pip install -r requirements.txt
streamlit run App.py
