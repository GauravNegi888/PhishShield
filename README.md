# 🛡️ PhishShield – Machine Learning Based Phishing URL Detection System

**PhishShield** is a cybersecurity web application designed to identify potentially malicious and phishing URLs using Machine Learning. It analyzes submitted website URLs and predicts whether they are likely to be **Safe or Phishing**, helping users make informed decisions before visiting unfamiliar websites.

The application uses a trained **Gradient Boosting Classifier** and URL feature extraction techniques to identify suspicious patterns and classify potentially dangerous websites.

PhishShield provides a modern, responsive web interface that allows users to scan URLs and receive instant prediction results.

---

## 📌 Problem Statement

Phishing attacks are one of the most common cybersecurity threats on the internet. Attackers create fraudulent websites that imitate legitimate platforms such as banking portals, social media websites, and e-commerce platforms to steal sensitive information.

These malicious websites often use URLs that closely resemble legitimate domains, making it difficult for ordinary users to identify phishing attempts manually.

**Problem:** There is a need for an intelligent and accessible system that can analyze website URLs and help users identify potentially malicious websites before accessing them.

**Solution:** PhishShield uses Machine Learning algorithms and URL feature extraction techniques to analyze submitted URLs and classify them as potentially legitimate or phishing. The results are displayed through a user-friendly web interface.

---

## 🎯 Project Objectives

- Detect potentially malicious and phishing URLs using Machine Learning.
- Extract meaningful features from submitted website URLs.
- Classify URLs using a trained Gradient Boosting Classifier.
- Provide users with instant prediction results.
- Display prediction confidence through an intuitive interface.
- Improve awareness about phishing attacks and online security.
- Develop a responsive and user-friendly cybersecurity application.

---

## ✨ Key Features

- **URL Scanning:** Users can enter a website URL for security analysis.
- **Machine Learning Detection:** Uses a trained Gradient Boosting Classifier to identify potentially malicious URLs.
- **URL Feature Extraction:** Analyzes URL characteristics and patterns to generate input features for the ML model.
- **Instant Results:** Displays the prediction immediately after URL analysis.
- **Prediction Confidence:** Shows a percentage associated with the model's prediction.
- **Modern User Interface:** Responsive dark-themed cybersecurity dashboard.
- **Security Warning:** Provides an additional confirmation before opening URLs classified as potentially suspicious.
- **User-Friendly Design:** Simple and intuitive interface for easy URL scanning.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Backend development and URL processing |
| Flask | Web application framework |
| Scikit-learn | Machine Learning model and prediction |
| Gradient Boosting Classifier | Phishing URL classification |
| NumPy | Numerical operations |
| Pandas | Dataset processing and analysis |
| HTML5 | Structure of the web application |
| CSS3 | Styling and responsive design |
| JavaScript | Frontend functionality and result visualization |
| Pickle | Saving and loading the trained ML model |
| Git & GitHub | Version control and collaboration |

---

## ⚙️ How It Works

1. **User Input:** The user enters a website URL into the PhishShield scanner.
2. **URL Processing:** The Flask backend receives the submitted URL.
3. **Feature Extraction:** The application extracts relevant characteristics from the submitted URL.
4. **Machine Learning Prediction:** The extracted features are passed to the trained Gradient Boosting Classifier.
5. **Classification:** The model predicts whether the submitted URL is likely safe or phishing.
6. **Result Generation:** The application generates a prediction and associated confidence percentage.
7. **Display:** The result is displayed through the web interface, allowing users to make informed browsing decisions.

---

## 🔍 URL Features for Analysis

PhishShield uses different URL characteristics to identify patterns commonly associated with phishing websites.

Some of the characteristics include:

- URL length
- Presence of IP addresses instead of domain names
- Number of subdomains
- Special characters in URLs
- Suspicious keywords and URL patterns
- Domain-related characteristics
- HTTPS and HTTP usage
- URL structure and formatting

These features are processed and used by the trained Machine Learning model to generate predictions.

---

## 🧠 Machine Learning Model

PhishShield uses a **Gradient Boosting Classifier** for phishing URL detection.

Gradient Boosting is an ensemble Machine Learning algorithm that combines multiple decision trees to generate predictions.

The trained model analyzes extracted URL features and classifies submitted URLs based on patterns learned from labelled training data.

The trained model is stored in Pickle format and loaded by the Flask application to perform predictions.

---

## 📂 Project Structure

```text
PhishShield/
│
├── app.py
│
├── feature.py
│
├── pickle/
│   └── model.pkl
│
├── static/
│   └── styles.css
│
├── templates/
│   └── index.html
│
├── phishing.csv
│
├── requirements.txt
│
├── Phishing URL Detection.ipynb
│
├── .gitignore
│
└── README.md
