# SMS-Spam-Detection
# 📩 SMS Spam Detection — NLP End-to-End Project

## 📌 Project Overview

This project implements a complete Natural Language Processing (NLP) pipeline to classify SMS messages as:

- **Spam** (unsolicited or malicious messages)
- **Ham** (legitimate messages)

The solution follows a structured AI development life cycle, including data preprocessing, feature engineering, model training, evaluation, and deployment using Streamlit.

The final model is deployed as an interactive web application.

---

## 🎯 Objectives

- Perform text preprocessing on raw SMS data  
- Convert text into numerical features using **TF-IDF vectorization**  
- Train and compare machine learning classifiers  
- Evaluate model performance using multiple metrics  
- Deploy the trained model using **Streamlit**  

---

## 🗂 Project Structure

ai-spam-detector/
│
├── app.py # Streamlit application
├── requirements.txt # Required Python packages
├── README.md # Project documentation
│
├── models/
│ └── spam_detector_calibrated_svm.joblib # Saved trained model
│
├── data/
│ └── sms_spam.csv # Dataset
│
├── report/
│ └── Spam_Detection_Report.pdf
│
└── slides/
└── Spam_Detection_Slides.pptx


---

## 🧠 Methodology

### 1️⃣ Data Collection
Dataset: SMS Spam Collection Dataset (UCI Machine Learning Repository)  
Contains labeled SMS messages (spam/ham).

### 2️⃣ Data Preprocessing
- Text cleaning  
- Lowercasing  
- Stopword removal  
- Tokenization  
- TF-IDF vectorization  

### 3️⃣ Model Training
Several classifiers were evaluated:
- Logistic Regression  
- Support Vector Machine (SVM)  
- Naive Bayes  

The best-performing model was selected based on:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  

### 4️⃣ Model Saving
The final trained model was saved using `joblib` for deployment.

### 5️⃣ Deployment
The model is deployed using **Streamlit**, allowing users to input SMS messages and receive real-time predictions.

---

## 📊 Model Evaluation

Performance was assessed using:

- Confusion Matrix  
- Classification Report  
- ROC Curve  
- Precision-Recall Curve  

Special attention was given to:
- False positives (ham classified as spam)
- False negatives (spam classified as ham)

---

## 🚀 How to Run Locally

### Step 1: Clone the repository

```bash
git clone https://github.com/your-username/ai-spam-detector.git
cd ai-spam-detector


Step 2: Install dependencies
pip install -r requirements.txt
Step 3: Run the Streamlit app
streamlit run app.py

The app will open in your browser.
