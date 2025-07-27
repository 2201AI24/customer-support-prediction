# 🛠 Customer Support Analytics: Satisfaction & Resolution Time Prediction

This project is an end-to-end ML solution that analyzes customer support tickets to predict customer satisfaction (classification) and resolution time (regression). Built with a user-friendly Streamlit interface, it allows users to upload CSVs, perform exploratory analysis, and generate predictions.

---

## 📌 Overview

The application ingests customer support ticket data, preprocesses it with rich feature engineering, and applies trained ML models to:

- Predict whether the customer will be **satisfied or unsatisfied**
- Estimate the **expected time to resolve** the support request

---

## 🚀 Features

* Classifies support satisfaction using an ensemble Voting Classifier
* Predicts resolution time using Linear Regression
* Extracts 290+ features using sentiment analysis (VADER, TextBlob), TF-IDF, and ticket metadata
* Visualizes data distribution, feature importance, and model results in Streamlit
* Interactive CSV upload with per-ticket insights

---

## 🛠️ Technologies Used

* Python
* Scikit-learn
* TextBlob & VADER
* Pandas & NumPy
* Streamlit
* Matplotlib & Seaborn
* Jupyter Notebook

---

## 🧠 Model Details

### Satisfaction Prediction:
* Model: Voting Classifier (Logistic Regression + Decision Tree + Random Forest)
* Metric: F1 Score – **56.3%**
* Features: Sentiment polarity, ticket urgency, TF-IDF vectors, categorical encodings

### Resolution Time Prediction:
* Model: Linear Regression
* Metric: MAE – **0.077 hours**, RMSE ~0.0106
* Notes: Temporal, categorical, and text features combined for high accuracy

---

## 📷 Streamlit Preview

![Screenshot](https://user-images.githubusercontent.com/your-placeholder-image-link-here.png) <!-- Replace or remove this if not available -->

---

## 📦 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/2201AI24/customer-support-prediction.git
   cd customer-support-prediction
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

---

## 📁 Project Structure

```
customer-support-prediction/
├── app/
│   └── app.py                  # Streamlit interface
├── models/
│   ├── satisfaction_model.pkl  # Voting Classifier
│   └── time_model.pkl          # Linear Regression
├── utils/
│   └── preprocessing.py        # Feature engineering & encoding
├── data/
│   └── sample_tickets.csv      # Example support data
├── requirements.txt
├── README.md
└── notebooks/
    └── model.ipynb      # Full pipeline development

```

---

## 👨‍💻 Author

M. Umesh Chandra<br>
BTech Artificial Intelligence and Data Science (Batch 2022)<br> 
Project: Telecom Churn Prediction + LLM Explanation

---

## 📄 License

This project is for educational use only.
