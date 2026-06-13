# AI-Based-Hiring-Prediction-System
Built an AI-based Hiring Prediction System using Machine Learning to classify candidates as Hired or Rejected based on resume data. Achieved 100% accuracy using Logistic Regression.
# AI-Based Hiring Prediction System

## Overview

The AI-Based Hiring Prediction System is an end-to-end Machine Learning project that predicts whether a candidate will be **Hired** or **Rejected** based on resume-related information such as skills, experience, education, certifications, projects, salary expectations, and AI assessment scores.

This project simulates a real-world AI-powered resume screening system used in recruitment and HR analytics to automate candidate evaluation and hiring decisions.

---

## Dataset Features

- Resume_ID
- Name
- Skills
- Experience (Years)
- Education
- Certifications
- Job Role
- Salary Expectation ($)
- Projects Count
- AI Score (0-100)
- Recruiter Decision (Target Variable)

### Target Variable

- Hire → 1
- Reject → 0

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Data Preprocessing
- Loaded dataset
- Checked missing values
- Removed unnecessary columns
- Encoded categorical features
- Feature scaling using StandardScaler

### 2. Exploratory Data Analysis
- Dataset statistics
- Correlation analysis
- Feature relationship visualization

### 3. Model Building
Implemented and compared:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest

### 4. Hyperparameter Tuning
- Applied GridSearchCV
- Optimized Logistic Regression parameters

### 5. Model Evaluation
Evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## Results

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 100% |
| Decision Tree | 100% |
| Random Forest | 100% |
| KNN | 94.5% |

### Best Model
**Logistic Regression**

- Accuracy: 100%
- Precision: 100%
- Recall: 100%
- F1 Score: 100%

---

## Feature Importance

The most influential features affecting hiring decisions include:

- AI Score
- Experience (Years)
- Projects Count
 

These factors showed the strongest correlation with recruiter decisions.

---

## Sample Prediction

```python
data = [[200, 5, 2, 1, 3, 70000, 6, 85]]

data_scaled = scaler.transform(data)

prediction = best_model.predict(data_scaled)

if prediction[0] == 1:
    print("Hired")
else:
    print("Rejected")
```

---

## Project Outcome

Successfully developed an AI-powered hiring prediction system capable of automatically screening candidates and predicting recruitment outcomes with high accuracy, helping streamline HR decision-making processes.

---

## Author

Hasini Macha

Machine Learning | AI | Data Science Enthusiast
