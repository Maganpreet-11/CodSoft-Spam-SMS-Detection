# 📧 Spam SMS Detection using Machine Learning

## 📖 Overview

Spam SMS messages are a major issue in digital communication, often containing advertisements, phishing attempts, fraudulent offers, and malicious links. Detecting such messages automatically can help users avoid scams and improve communication security.

This project develops a Machine Learning-based Spam SMS Detection System capable of classifying SMS messages as either:

- **Spam** – Unwanted or fraudulent messages
- **Ham** – Legitimate messages

The project uses **Natural Language Processing (NLP)** techniques and **Machine Learning algorithms** to analyze text messages and make accurate predictions.

Developed as part of the **CodSoft Machine Learning Internship**.

---

## 🎯 Objectives

The primary objectives of this project are:

- Build an intelligent SMS classification system.
- Apply Natural Language Processing techniques.
- Convert textual data into numerical features.
- Train a Machine Learning model for binary classification.
- Evaluate model performance using industry-standard metrics.
- Save the trained model for future deployment.

---

## 🗂 Dataset Information

The dataset contains SMS messages labeled as either spam or ham.

### Features

| Column | Description |
|----------|-------------|
| label | SMS category (Spam/Ham) |
| message | SMS text content |

### Example Records

| Label | Message |
|---------|---------|
| Ham | Hey, are we meeting tomorrow? |
| Spam | Congratulations! You've won a free prize. Click now! |

---

## 🛠 Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Scikit-learn
- Pickle

### Machine Learning
- Logistic Regression

### NLP Techniques
- Text Cleaning
- TF-IDF Vectorization

---

## ⚙️ Project Workflow

### 1. Data Collection

The SMS dataset is loaded and inspected for:

- Missing values
- Duplicate records
- Class distribution

---

### 2. Data Preprocessing

The text data undergoes preprocessing to improve model performance.

Steps include:

- Removing unnecessary columns
- Converting labels into numerical values
- Removing duplicates
- Cleaning text where required

---

### 3. Feature Engineering

Machine Learning algorithms cannot directly understand text data.

Therefore, messages are converted into numerical vectors using:

### TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) assigns importance scores to words based on:

- Frequency within a message
- Rarity across the dataset

This helps the model focus on meaningful words.

---

### 4. Train-Test Split

The dataset is divided into:

| Dataset | Percentage |
|----------|------------|
| Training Data | 80% |
| Testing Data | 20% |

This ensures unbiased model evaluation.

---

### 5. Model Training

The classification model is trained using:

### Logistic Regression

Why Logistic Regression?

✔ Fast Training

✔ High Accuracy

✔ Efficient for Binary Classification

✔ Excellent Performance on Text Data

---

### 6. Model Evaluation

The model is evaluated using:

#### Accuracy

Measures overall prediction correctness.

#### Precision

Measures how many predicted spam messages were actually spam.

#### Recall

Measures how many actual spam messages were correctly detected.

#### F1 Score

Balances precision and recall.

#### Confusion Matrix

Provides detailed classification insights.

---

### 7. Model Saving

The trained model and TF-IDF vectorizer are saved using Pickle files.

Generated files:

```text
spam_model.pkl
spam_tfidf.pkl
```

These files can be reused without retraining the model.

---

## 📁 Project Structure

```text
CodSoft-Spam-SMS-Detection/
│
├── spam.csv
├── model.ipynb
├── spam_model.pkl
├── spam_tfidf.pkl
├── README.md
├── requirements.txt
│
└── images/
```

---

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/CodSoft-Spam-SMS-Detection.git
```

### Navigate to Project Folder

```bash
cd CodSoft-Spam-SMS-Detection
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶ Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
model.ipynb
```

Run all cells sequentially.

---

## 🧪 Testing the Model

Example:

```python
msg1 = "Congratulations! You have won 10000 rupees. Click the link now."

msg2 = "Hey bro, are you coming to college tomorrow?"

print(predict_sms(msg1))
print(predict_sms(msg2))
```

### Output

```text
SPAM
HAM
```

---

## 📊 Machine Learning Pipeline

```text
SMS Messages
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

Through this project, the following concepts were learned and implemented:

- Data Cleaning
- Text Preprocessing
- Natural Language Processing
- Feature Engineering
- TF-IDF Vectorization
- Machine Learning Classification
- Model Evaluation
- Model Serialization
- Real-world Spam Detection Systems

---

## 🔮 Future Improvements

Potential enhancements include:

- Deep Learning Models (LSTM, GRU, BERT)
- Streamlit Web Application
- Flask API Deployment
- Real-time SMS Classification
- Multi-language Spam Detection
- Hyperparameter Optimization

---

## 🎖 CodSoft Machine Learning Internship

This project was completed as part of the **CodSoft Machine Learning Internship Program**.

The internship focuses on developing practical Machine Learning solutions and applying AI concepts to real-world problems.

Project Domain:
- Machine Learning
- Natural Language Processing
- Text Classification

---

## 👨‍💻 Author

### Maganpreet Singh

B.Tech Computer Science Student

Interested in:
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Data Science

GitHub: https://github.com/yourusername

---

## 📜 License

This project is intended for educational and learning purposes under the CodSoft Machine Learning Internship Program.

Feel free to fork, modify, and learn from the project.
