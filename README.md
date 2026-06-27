# 🤖 NLP Intent Classification Chatbot

An AI-powered chatbot that classifies user intents across multiple categories using NLP and Logistic Regression, deployed as a Streamlit web application with persistent multi-turn conversation history.

---

## 📌 Overview

This chatbot goes beyond simple keyword matching — it uses NLP preprocessing and machine learning to understand the *intent* behind a user's message, enabling accurate, context-aware responses across a wide range of categories.

**Key capabilities:**
- Multi-category intent classification using NLP + Logistic Regression
- Persistent conversation history across the session
- Real-time multi-turn interaction via Streamlit interface
- Text preprocessing pipeline: tokenization, vectorization, feature engineering

---

## 🛠 Tech Stack

| Component | Technology |
|---|---|
| Intent Classification | Logistic Regression (Scikit-learn) |
| NLP Pipeline | Tokenization · TF-IDF · Text Preprocessing |
| Frontend | Streamlit |
| Data | Custom intents JSON (patterns + responses) |
| Language | Python |

---

## 🏗 Architecture

```
User Message
      ↓
Text Preprocessing (Tokenization → TF-IDF Vectorization)
      ↓
Logistic Regression Intent Classifier
      ↓
Intent → Response Mapping (intents.json)
      ↓
Streamlit UI with Conversation History Log
```

---

## ⚙️ How to Run Locally

```bash
# Clone the repo
git clone https://github.com/Sudha0626/Chatbot-using-nlp-Aicte.git
cd Chatbot-using-nlp-Aicte

# Install dependencies
pip install streamlit scikit-learn nltk numpy

# Run the app
streamlit run chatbot.py
```

---

## 📁 Project Structure

```
Chatbot-using-nlp-Aicte/
├── chatbot.py          # Main Streamlit app + model logic
├── intents.json        # Intent patterns and responses dataset
├── requirements.txt
└── README.md
```

---

## 📊 Sample Intents

The model classifies messages into categories such as:
- Greetings / Farewells
- Help requests
- Product/service queries
- General conversation

---

## 🌱 Future Improvements

- Replace Logistic Regression with a fine-tuned BERT model for higher accuracy
- Add multi-language support
- Integrate with a backend API for dynamic intent management

---
👩‍💻 Author

Raaga Sudha — LinkedIn: https://www.linkedin.com/in/raagasudha06/ · Github: https://github.com/Sudha0626/

Built during AI & Data Analytics Internship at AICTE-Shell Edunet Foundation, Chennai (Jan–Feb 2025)

