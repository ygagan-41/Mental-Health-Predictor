# 🧠 Mental Health Predictor

### Student Wellness Analytics using Machine Learning + FastAPI

A machine-learning-powered web application that analyzes **academic habits, digital behavior, lifestyle patterns, and perceived stress** to generate an estimated mental-health score.

🔗 **Live Demo:**
[https://mental-health-predictor-7wb3.onrender.com/]

---

## 📌 About the Project

The **Mental Health Predictor** is an end-to-end machine learning project designed to explore how everyday lifestyle and digital habits may be associated with mental-health indicators.

The application collects information such as:

* 👤 Age
* ⚧️ Gender
* 🌍 Country
* 🎓 Academic level
* 📱 Most-used social/digital platform
* 💻 Primary platform usage purpose
* ⏱️ Daily screen time
* 📲 Daily phone unlocks
* 📚 Study hours per day
* 🏃 Physical activity
* 😴 Sleep duration
* 😟 Perceived stress level

The trained machine learning model processes these features and produces an estimated **mental-health score from 0–10**.

---

## 🌐 Live Application

Try the deployed application here:

👉 [Mental Health Predictor — Live Demo](https://mental-health-predictor-7wb3.onrender.com/)

The application provides a simple interface where users can enter their information and receive a predicted score.

---

## ✨ Features

* 🧠 Machine-learning-based prediction
* 🌐 REST API powered by FastAPI
* 🎨 Simple and responsive web interface
* 📊 Handles numerical and categorical features
* 🌍 Supports multiple countries
* 📱 Considers digital habits and screen usage
* 😴 Includes sleep and physical activity patterns
* 😟 Includes perceived stress level
* 🚀 Deployed online using Render
* 🔄 API-based prediction architecture

---

## 🏗️ Project Architecture

```text
User
 │
 ▼
Web Interface
 │
 ▼
FastAPI Backend
 │
 ├── Input Validation
 │
 ├── Data Preprocessing
 │
 └── Machine Learning Model
          │
          ▼
    Prediction / Score
          │
          ▼
      Web Interface
```

---

## 🛠️ Tech Stack

| Technology                 | Purpose                   |
| -------------------------- | ------------------------- |
| 🐍 Python                  | Core programming language |
| 🤖 Scikit-learn            | Machine learning          |
| 🐼 Pandas                  | Data processing           |
| 🔢 NumPy                   | Numerical operations      |
| ⚡ FastAPI                  | Backend API               |
| 📦 Pydantic                | Request validation        |
| 🔐 Joblib                  | Model serialization       |
| 🌐 HTML / CSS / JavaScript | Frontend                  |
| 🚀 Render                  | Deployment                |
| 🐙 Git & GitHub            | Version control           |

---

## 🤖 Machine Learning Workflow

The project follows a typical machine-learning pipeline:

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Feature Engineering
     │
     ▼
Categorical Encoding
     │
     ▼
Feature Scaling / Preprocessing
     │
     ▼
Model Training
     │
     ▼
Model Evaluation
     │
     ▼
Model Serialization
     │
     ▼
FastAPI Integration
     │
     ▼
Deployment
```

---

## 🔍 Input Features

The model uses a combination of demographic, academic, digital, lifestyle, and stress-related features.

### Profile

* Age
* Gender
* Country

### Academic & Digital Habits

* Academic level
* Most-used platform
* Primary purpose of platform usage
* Average daily screen time
* Daily phone unlocks

### Lifestyle & Stress

* Study hours per day
* Physical activity per day
* Sleep per night
* Perceived stress level

The deployed interface currently exposes these inputs directly to the user.

---

## 📊 Prediction

After submitting the form, the application generates a predicted **mental-health score between 0 and 10**.

Example:

```text
Predicted Mental Health Score

        7.4 / 10
```

The score should be interpreted only as a **machine-learning prediction**, not as a medical diagnosis.

---

## ⚡ FastAPI API

The backend is built using **FastAPI**.

A typical prediction request follows this architecture:

```text
POST /predict
       │
       ▼
Validate Input
       │
       ▼
Preprocess Features
       │
       ▼
Load ML Model
       │
       ▼
Generate Prediction
       │
       ▼
Return Result
```

Example response:

```json
{
    "prediction": 7.4
}
```

> The exact API response may vary depending on the implementation of the current backend.

---

## 📁 Project Structure

A possible project structure is:

```text
Mental-Health-Predictor/
│
├── app.py
├── model/
│   ├── Mental_Health_Model.pkl
│   ├── scaler.pkl
│   └── columns.pkl
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── dataset/
│   └── dataset.csv
│
├── requirements.txt
├── README.md
└── .gitignore

```
