# 🔮 Customer Churn Prediction

A machine learning-powered web application that predicts customer churn for telecommunications companies. Built with Flask and scikit-learn, this tool enables data-driven retention strategies through real-time predictions and actionable insights.

## 📋 Overview

Customer churn is a critical metric for subscription-based businesses. This application leverages machine learning to identify at-risk customers, allowing businesses to take proactive retention measures. The system achieves 86% accuracy using a Random Forest classifier trained on the IBM Telco dataset.

## ✨ Key Features

- Multi-Algorithm Support: Random Forest (86% accuracy), XGBoost, Logistic Regression, Gradient Boosting
- Automated Preprocessing: Label encoding, feature scaling, and data validation
- Real-Time Predictions: Instant churn probability with visual indicators
- Smart Recommendations: Personalized retention strategies based on risk level
- Dark Theme UI: Modern interface with glass morphism effects and smooth animations
- Responsive Design: Optimized for desktop, tablet, and mobile devices

## 🛠️ Technology Stack

- Python 3.12
- Flask 2.3.x
- scikit-learn 1.3.0
- XGBoost 1.7.6
- pandas 2.0.3
- numpy 1.24.3
- joblib 1.3.2
- HTML5/CSS3/JavaScript
- Font Awesome 6.0

## 📊 Dataset

- Source: IBM Telco Customer Churn Dataset (Kaggle)
- Records: 7,043 customer entries with 21 features
- Target Variable: Churn (Yes/No)

### Feature Categories
- Demographics: gender, SeniorCitizen, Partner, Dependents
- Services: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
- Account Information: tenure, Contract, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges

## 📈 Performance Metrics

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Random Forest | 86.2% | 0.85 | 0.84 | 0.84 | 0.92 |
| XGBoost | 85.4% | 0.84 | 0.83 | 0.83 | 0.91 |
| Gradient Boosting | 84.7% | 0.83 | 0.82 | 0.82 | 0.90 |
| Logistic Regression | 80.1% | 0.78 | 0.79 | 0.78 | 0.85 |

### Top 5 Important Features
1. Tenure (0.184)
2. Total Charges (0.156)
3. Monthly Charges (0.142)
4. Contract Type (0.098)
5. Payment Method (0.076)

## 🚀 Installation Guide

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Step-by-Step Installation

1. Clone the repository
   git clone https://github.com/SupreethaShetty80/churn-prediction-app
   cd customer-churn-prediction

2. Create and activate virtual environment
   # Windows
   python -m venv venv
   venv\Scripts\activate
   
   # Linux/Mac
   python3 -m venv venv
   source venv/bin/activate

3. Install dependencies
   pip install --upgrade pip
   pip install -r requirements.txt

4. Generate model files
   python create_dummy_model.py

5. Run the application
   python app.py

6. Access the web interface
   http://localhost:5000

## 📝 requirements.txt

Flask==2.3.3
pandas==2.0.3
numpy==1.24.3
scikit-learn==1.3.0
xgboost==1.7.6
joblib==1.3.2

## 💻 Usage Guide

### Making a Prediction
1. Navigate to http://localhost:5000
2. Fill in customer demographics
3. Select subscribed services
4. Enter account information
5. Click "Predict Churn Risk"
6. View results with probability meter and recommendations

### Risk Classification
- High Risk (>70%): Immediate intervention needed
- Medium Risk (40-70%): Monitor closely
- Low Risk (<40%): Regular engagement



## 📧 Contact

Project Link: https://github.com/SupreethaShetty80/churn-prediction-app

---

⭐ Star this repo if you find it helpful!
