# 📧 Spam SMS Detection using Machine Learning

## 📌 Project Overview

Spam SMS Detection is a Machine Learning project developed as part of the **CodSoft Machine Learning Internship**. The goal of this project is to classify SMS messages as either **Spam** or **Ham (Legitimate)** using Natural Language Processing (NLP) and Machine Learning techniques.

The model analyzes the content of SMS messages and predicts whether a message is unwanted spam or a genuine message.

---

## 🎯 Objectives

- Build a machine learning model for SMS classification.
- Apply Natural Language Processing techniques to text data.
- Convert text into numerical features using TF-IDF.
- Train and evaluate a classification model.
- Save the trained model for future use and deployment.

---

## 🗂 Dataset

The dataset contains SMS messages labeled as:

| Label | Description |
|---------|-------------|
| Ham | Legitimate SMS message |
| Spam | Unwanted or promotional SMS message |

### Sample Messages

**Ham**

```text
Hey, are we meeting tomorrow?
```

**Spam**

```text
Congratulations! You have won ₹10,000. Click the link now.
```

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TF-IDF Vectorizer
- Pickle
- Jupyter Notebook

---

## 🔄 Project Workflow

### 1. Data Loading
The SMS dataset is loaded and inspected for quality.

### 2. Data Preprocessing
- Handle missing values
- Remove duplicates
- Encode labels
- Prepare text data

### 3. Feature Extraction
TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert SMS text into numerical vectors.

### 4. Model Training
A Logistic Regression classifier is trained on the processed data.

### 5. Model Evaluation
The model is evaluated using:
- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- Confusion Matrix

### 6. Model Saving
The trained model and TF-IDF vectorizer are saved using Pickle for future predictions.

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression was chosen because:

- Effective for binary classification
- Fast training and prediction
- Performs well on text classification tasks
- Easy to deploy

---

## 📁 Project Structure

```text
CodSoft-Spam-SMS-Detection/
│
├── spam.csv
├── model.ipynb
├── spam_model.pkl
└── spam_tfidf.pkl
```

### File Description

#### spam.csv
Dataset containing SMS messages and their labels.

#### model.ipynb
Jupyter Notebook containing:
- Data preprocessing
- TF-IDF vectorization
- Model training
- Model evaluation
- Prediction examples

#### spam_model.pkl
Saved trained Logistic Regression model.

#### spam_tfidf.pkl
Saved TF-IDF vectorizer used during prediction.

---

## 🚀 How to Run

### Clone the Repository

```bash
git clone https://github.com/yourusername/CodSoft-Spam-SMS-Detection.git
```

### Navigate to the Project Directory

```bash
cd CodSoft-Spam-SMS-Detection
```

### Open Jupyter Notebook

```bash
jupyter notebook
```

### Run

Open:

```text
model.ipynb
```

Run all cells sequentially.

---

## 🧪 Example Prediction

```python
msg1 = "Congratulations! You have won 10000 rupees. Click the link now."

msg2 = "Hey bro, are you coming to college tomorrow?"
```

### Output

```text
SPAM

HAM
```

---

## 📊 Model Pipeline

```text
SMS Message
     │
     ▼
Text Preprocessing
     │
     ▼
TF-IDF Vectorization
     │
     ▼
Logistic Regression
     │
     ▼
Prediction
     │
     ▼
Spam / Ham
```

---

## 🎓 Learning Outcomes

This project helped in understanding:

- Machine Learning Fundamentals
- Text Classification
- Natural Language Processing
- TF-IDF Vectorization
- Logistic Regression
- Model Evaluation
- Model Serialization with Pickle

---

## 🔮 Future Improvements

- Deploy using Streamlit
- Build a Flask API
- Use Deep Learning Models (LSTM/BERT)
- Real-time SMS Classification
- Multi-language Support

---

## 🎖 CodSoft Machine Learning Internship

This project was completed as part of the **CodSoft Machine Learning Internship Program**, focusing on practical implementation of Machine Learning techniques to solve real-world problems.

---

## 👨‍💻 Author

**Maganpreet Singh**

B.Tech Computer Science Student  
Machine Learning & AI Enthusiast

---

## ⭐ If you found this project useful, consider giving it a star!
