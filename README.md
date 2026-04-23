# 📧 Email Scam Detection using Multiple Machine Learning Algorithms

## 📌 Overview

This project builds a robust **Email Scam Detection System** using a wide range of Machine Learning algorithms. The goal is to classify emails as **Scam (Phishing/Spam)** or **Legitimate (Ham)** by leveraging multiple models and comparing their performance.

---

## 🚀 Features

* Supports **multiple ML algorithms** for comparison
* Text preprocessing and feature engineering pipeline
* Model training, evaluation, and selection
* Performance comparison across models
* Scalable and modular code structure

---

## 🧠 Algorithms Used

This project implements and compares the following models:

* Logistic Regression
* Support Vector Machine (SVM)
* Naive Bayes (MultinomialNB)
* Decision Tree
* K-Nearest Neighbors (KNN)
* Random Forest
* AdaBoost
* Bagging Classifier
* Extra Trees Classifier
* Gradient Boosting
* XGBoost

---

## 🔄 Machine Learning Pipeline

### 1. Data Preprocessing

* Lowercasing text
* Removing punctuation and special characters
* Tokenization
* Stopword removal
* Stemming / Lemmatization

### 2. Feature Extraction

* Bag of Words (BoW)
* TF-IDF (Term Frequency–Inverse Document Frequency)

### 3. Model Training

Each algorithm is trained on the same dataset and evaluated using consistent metrics for fair comparison.

---

## 📂 Project Structure

```bash
email-scam-detection/
│
├── data/
│   ├── raw_emails.csv
│   └── processed_data.csv
│
├── notebooks/
│   └── model_comparison.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── train_models.py
│   ├── evaluate.py
│   └── predict.py
│
├── models/
│   ├── logistic_regression.pkl
│   ├── svm.pkl
│   ├── naive_bayes.pkl
│   ├── random_forest.pkl
│   └── best_model.pkl
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/email-scam-detection.git
cd email-scam-detection
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### Train All Models

```bash
python src/train_models.py
```

### Evaluate Models

```bash
python src/evaluate.py
```

### Make Predictions

```bash
python src/predict.py --text "Urgent! Your account has been compromised. Click here to secure it."
```

---

## 📊 Evaluation Metrics

Each model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## 📈 Model Comparison (Example)

| Model               | Accuracy | Precision | Recall | F1-score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.95     | 0.94      | 0.96   | 0.95     |
| SVM                 | 0.96     | 0.95      | 0.97   | 0.96     |
| Naive Bayes         | 0.93     | 0.92      | 0.94   | 0.93     |
| Random Forest       | 0.97     | 0.96      | 0.98   | 0.97     |
| XGBoost             | 0.98     | 0.97      | 0.99   | 0.98     |

---

## 🧪 Code Snippet (Models Initialization)

```python
from sklearn.linear_model import LogisticRegression
from sklearn.svm import SVC
from sklearn.naive_bayes import MultinomialNB
from sklearn.tree import DecisionTreeClassifier
from sklearn.neighbors import KNeighborsClassifier
from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier, BaggingClassifier, ExtraTreesClassifier, GradientBoostingClassifier
from xgboost import XGBClassifier

models = {
    "Logistic Regression": LogisticRegression(),
    "SVM": SVC(),
    "Naive Bayes": MultinomialNB(),
    "Decision Tree": DecisionTreeClassifier(),
    "KNN": KNeighborsClassifier(),
    "Random Forest": RandomForestClassifier(),
    "AdaBoost": AdaBoostClassifier(),
    "Bagging": BaggingClassifier(),
    "Extra Trees": ExtraTreesClassifier(),
    "Gradient Boosting": GradientBoostingClassifier(),
    "XGBoost": XGBClassifier()
}
```

---

## 🛠️ Tech Stack

* Python
* Scikit-learn
* XGBoost
* Pandas
* NumPy
* NLTK / spaCy
* Matplotlib / Seaborn

---

## 🔐 Use Cases

* Email spam filtering systems
* Phishing detection tools
* Enterprise cybersecurity solutions
* Personal email protection

---

## ⚠️ Limitations

* Performance varies with dataset quality
* May struggle with highly sophisticated phishing emails
* Requires regular updates with new data

---

## 🔮 Future Improvements

* Deep Learning models (LSTM, BERT)
* Real-time API deployment
* Integration with email clients
* Multilingual scam detection

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 📬 Contact

For questions or suggestions, open an issue on GitHub.

---
