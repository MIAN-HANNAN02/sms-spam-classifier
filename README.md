# SMS Spam Classifier 📱

A Machine Learning web application that classifies SMS messages as either **Spam** or **Ham** (Not Spam). This project uses Natural Language Processing (NLP) to process text and a classification model to predict the nature of the message. 

### 🔴 Live Demo
Check out the live web app here: https://sms-spam-classifier-m8idw7zqywfxgwkz9qwlp7.streamlit.app/

---

## 🛠️ Features
* **Real-time Classification:** Type or paste an SMS message and get an instant prediction.
* **NLP Pipeline:** Includes text cleaning, tokenization, stop-word removal, and stemming using NLTK.
* **Interactive UI:** Built with Streamlit for a clean, user-friendly web interface.

## 💻 Tech Stack
* **Language:** Python
* **Machine Learning:** Scikit-learn
* **NLP:** NLTK (Natural Language Toolkit)
* **Data Manipulation:** Pandas, NumPy
* **Web Framework:** Streamlit
* **Deployment:** Streamlit Cloud & GitHub

---

## ⚙️ How It Works
1. **Preprocessing:** The input text is converted to lowercase, stripped of special characters/punctuation, and broken down into individual words (tokenization). Stop words are removed, and the remaining words are stemmed.
2. **Vectorization:** The cleaned text is converted into numerical data using TF-IDF (Term Frequency-Inverse Document Frequency) or Bag of Words.
3. **Prediction:** The vectorized text is passed to the trained Machine Learning model , which outputs a Spam or Ham classification.

---

## 📂 Project Structure
```text
├── app.py                 # Main Streamlit application code
├── setup.sh               # Shell script for automated environment setup
├── model.pkl              # Saved Machine Learning model
├── vectorizer.pkl         # Saved text vectorizer (TF-IDF/CountVectorizer)
├── spam.csv               # Dataset used for training
├── requirements.txt       # List of Python dependencies
└── README.md              # Project documentation
