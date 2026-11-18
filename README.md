# 🩺 AI-Health-Chatbot 🌐💡

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange?logo=scikit-learn&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Symptom%20Extraction-green)
![Web Framework](https://img.shields.io/badge/Web%20App-Flask%20%7C%20HTML%2FCSS-lightgrey?logo=flask&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

Ever wondered if Artificial Intelligence can act like a virtual healthcare assistant? 🤔 In this project, I built an end-to-end **AI-Powered Healthcare Chatbot** that predicts diseases from user-described symptoms using Machine Learning and Natural Language Processing (NLP) in Python, integrated with an interactive web interface for real-time consultations! 🚑💻

---

## 📋 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Project Architecture & Workflow](#project-architecture--workflow)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [Running the Application](#running-the-application)
- [Learning Outcomes](#learning-outcomes)
- [Medical Disclaimer](#medical-disclaimer)
- [License](#license)

---

## 🔍 Overview
Early symptom assessment helps individuals make informed decisions about seeking timely medical care. This repository implements a conversational healthcare assistant capable of understanding free-text symptom descriptions, asking dynamic follow-up questions to narrow down possibilities, predicting potential conditions with confidence scores, and offering actionable health precautions.

---

## ✨ Key Features
- **Symptom Extraction with NLP:** Parses and maps natural language user inputs to structured medical symptom features.
- **Machine Learning Disease Prediction:** Powered by a **Random Forest Classifier** trained on symptom-disease datasets for accurate multi-class classification.
- **Interactive Follow-Up Engine:** Dynamically asks clarifying questions about related symptoms to refine diagnostic confidence.
- **Confidence Scoring:** Displays probability/confidence scores alongside predicted conditions so users understand prediction certainty.
- **Actionable Health Guidance:** Provides tailored health tips, standard precautions, and supportive advice based on the predicted outcome.
- **Real-Time Web Interface:** Clean, responsive frontend connected to a Python backend for seamless browser-based interaction.

---

## 🛠️ Tech Stack
- **Programming Language:** Python 3.8+
- **Machine Learning & Data Science:** Scikit-learn (Random Forest), Pandas, NumPy
- **Natural Language Processing (NLP):** NLTK / Regex / TF-IDF / Fuzzy Matching
- **Backend & Web Framework:** Flask
- **Frontend:** HTML5, CSS3, JavaScript

---

## ⚙️ Project Architecture & Workflow
1. **User Input:** The user types their symptoms naturally into the web chat interface.
2. **NLP Processing:** The text is cleaned, tokenized, and matched against known symptom vectors.
3. **Dynamic Follow-Up:** The bot queries additional co-occurring symptoms to improve prediction accuracy.
4. **ML Inference:** The trained Random Forest model evaluates the final symptom vector and outputs the top disease prediction with its confidence score.
5. **Care Recommendations:** Relevant precautions, descriptions, and wellness tips are returned to the user.

---

## 📁 Project Structure
```text
AI-Health-Chatbot/
│
├── data/                       # Medical symptom & precaution datasets (.csv)
├── models/                     # Trained Random Forest model & label encoders (.pkl)
├── static/                     # CSS stylesheets, JS scripts, and UI assets
├── templates/                  # HTML templates for the Flask web interface
│   └── index.html
├── notebooks/                  # Data exploration & model training notebooks
├── app.py                      # Main Flask application and chatbot routing
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
