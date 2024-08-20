# Email Spam Detection Using Machine Learning

<div align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1400/1*_igArwmR7Pj_Mu_KUGD1SQ.png" alt="Email Spam Detection" width="600">
</div>

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [About Data](#about-data)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)

- [Conclusion](#conclusion)


## Introduction
Email is essential for communication, but spam emails create problems. This project focuses on developing better ways to detect spam using machine learning techniques.

## Problem Statement
Spam emails disrupt effective communication and pose security risks. Traditional methods struggle to keep up with evolving spam tactics. This project aims to use Python-based text classification techniques to accurately identify and classify spam emails, evaluating the performance through metrics such as accuracy, time, and error rate using algorithms like Naive Bayes, Multinomial Naive Bayes, and SVM.

## Objectives
- Develop and evaluate machine learning models for accurately classifying spam emails
- Use algorithms like Naive Bayes and SVM
- Compare model performance based on accuracy, time, and error rates
- Identify the most effective algorithm for spam detection

## About Data
- **Dataset Name**: Email Spam Classification Dataset CSV
- **Source**: Simplilearn
- **Size**: Over 5,000 email records
- **Columns**: 
  - Category (spam/ham)
  - Message (email content)
- **Link**: [Email Datasets](https://www.kaggle.com/datasets/venky73/spam-mails-dataset)

## Project Structure
1. Data Load
2. Data Preprocessing
3. EDA Analysis
4. Summary Statistics for Ham and Spam
5. Data Visualization
6. Model Training
7. Feature Selection
8. Splitting the Dataset
9. Feature Extraction
10. Model Fitting
11. Model Evaluation
12. Model Testing
13. Comparison with Other Models

## Installation
To set up the project environment, follow these steps:

1. Clone the repository
2. Create a virtual environment 
3. Install the required packages
4. The `requirements.txt` file should include
5. Download  data

## Usage
To run the project:

Ensure you're in the project directory and your virtual environment is activated (if used).
Run the main script:
```
 Email Span/Ham Detection Full End-to-End Machine Learning Project. ipynb
```
The script will:

- Load and preprocess the data
- Perform EDA and display visualizations
- Train the models
- Evaluate and compare model performance
  
To use the trained model for prediction script:
```
from spam_detector import SpamDetector

detector = SpamDetector()
detector.load_model('best_model.pkl')

email_text = "Your email content here"
prediction = detector.predict(email_text)
print(f"The email is classified as: {prediction}")
```
## Conclusion
- Support Vector Classifier (SVC) and Random Forest (RF) demonstrated the highest accuracy, both achieving approximately 97%,96% etc.

- Naive Bayes (NB) achieved a perfect precision score, indicating zero false positives.

- Other models, including Gradient Boosting, Adaboost, Logistic Regression, and Bagging Classifier, displayed competitive performance with accuracy scores ranging from 94.68% to 96.03%.

- The selection of the optimal model should consider factors beyond just accuracy, such as computational efficiency and the specific requirements of the application. It is advisable to perform further model fine-tuning and validation before making a final choice.

