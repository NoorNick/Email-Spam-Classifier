# 📧 Email Spam Classifier
A simple machine learning project to classify emails as Spam or Not Spam using Naive Bayes and TF-IDF vectorization.
<br><br>
## 🚀 Project Overview
This project builds a basic spam email classifier that uses text processing and the Multinomial Naive Bayes algorithm to identify whether an email is spam or not. It demonstrates core NLP preprocessing steps and classification techniques using Python's scikit-learn library.
<br><br>

## 🛠️ Features
- Preprocessing with TF-IDF vectorization (including unigrams & bigrams)

- Spam classification using Multinomial Naive Bayes

- Model training and testing on a small custom dataset

- Prediction and confidence scores on new email examples
<br><br>

## 🧰 Technologies Used
- Python 3.x

- scikit-learn

- pandas

- numpy
<br><br>

## 🗂️ Dataset
The dataset is a small handcrafted list of emails labeled as Spam (1) or Not Spam (0):

```
# Examples of spam emails
"Get rich quick! Buy now!", "Win a free iPhone today!", "Congratulations! You've won!", etc.

# Examples of not spam emails
"Meeting at 3pm tomorrow", "Project deadline reminder", "Team lunch next week", etc.
```

⚙️ Installation & Setup
1. Clone the repo:

```
git clone https://github.com/yourusername/email-spam-classifier.git
cd email-spam-classifier
```

2. (Optional) Create and activate a virtual environment:

```
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
```

3. Install required packages:

```
pip install -r requirements.txt
```
<br><br>

## ▶️ How to Run
Run the notebook or script to train the spam classifier and test it:

```
python spam_classifier.py
```
The script will:

- Train the model on the provided email dataset

- Evaluate and print accuracy and classification report

- Predict new example emails and show spam/not spam labels with confidence scores
<br><br>

## 📊 Sample Output
```
Accuracy: 1.0

Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00         1
           1       1.00      1.00      1.00         1

    accuracy                           1.00         2
   macro avg       1.00      1.00      1.00         2
weighted avg       1.00      1.00      1.00         2

Email: Congratulations! You've won a prize!
Prediction: Spam
Confidence: 99.99%

Email: Team meeting scheduled for Friday
Prediction: Not Spam
Confidence: 99.99%
```
