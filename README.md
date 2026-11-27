# 🚀 OIBSIP — Oasis Infobyte Student Internship Program

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data-150458?logo=pandas&logoColor=white)
![Internship](https://img.shields.io/badge/Oasis%20Infobyte-Data%20Science-blue)

Hi, I'm **[Your Name]** 👋
This repository contains all my work for the **Data Science track** of the **Oasis Infobyte Student Internship Program (SIP)**. Each project is a complete, end-to-end machine learning workflow: data loading, exploratory analysis, visualisation, modelling, evaluation and written conclusions.

---

## 📂 Projects

| # | Project | Type | Best Model | Key Result | Folder |
|---|---------|------|------------|-----------|--------|
| 1 | 🌸 **Iris Flower Classification** | Multi-class classification | K-Nearest Neighbours | 100% test accuracy, 97.3% 5-fold CV | [`DataScience-Task1-IrisClassification`](./DataScience-Task1-IrisClassification) |
| 4 | 📧 **Spam Detection** | NLP / binary classification | Linear SVM | F1 = 0.912, recall = 90.8% | [`DataScience-Task4-SpamDetection`](./DataScience-Task4-SpamDetection) |
| 5 | 📈 **Sales Prediction** | Regression | Polynomial Regression (deg 2) | R² = 0.987, MAE = 0.53 | [`DataScience-Task5-SalesPrediction`](./DataScience-Task5-SalesPrediction) |

> Task numbers follow the official Oasis Infobyte task list.

---

## 🔍 Project Highlights

### 1. 🌸 Iris Flower Classification
Predicts the species of an iris flower (*Setosa*, *Versicolor*, *Virginica*) from sepal and petal measurements.
- Full EDA with pairplot, box plots and a correlation heatmap
- Identified **petal length and petal width** as the most discriminative features
- Compared 4 models: Logistic Regression, KNN, Decision Tree, Random Forest
- Used **5-fold cross-validation** alongside the test split, because a 30-sample test set is too small to rank models reliably

### 2. 📧 Spam Detection
Classifies messages as spam or ham using an NLP pipeline.
- Preprocessing: lowercasing, punctuation removal, stopword removal, stemming
- Removed **403 duplicate messages** before splitting to prevent train/test leakage
- **TF-IDF** features (unigrams and bigrams) feeding Naive Bayes, Logistic Regression and Linear SVM
- Shows why **accuracy is misleading** on imbalanced data (about 87% ham) and why recall and F1 matter
- Bonus: word clouds for spam vs ham vocabulary

### 3. 📈 Sales Prediction
Predicts product sales from advertising spend on TV, Radio and Newspaper.
- Linear Regression baseline (R² = 0.90) vs Polynomial Regression (R² = 0.987) and Random Forest (R² = 0.982)
- The large jump from the baseline suggests the channels **reinforce each other** (interaction effects)
- Insight: **TV** drives the most overall variation, **Radio** gives the most sales per dollar, and **Newspaper** has almost no effect

---

## 🛠️ Tech Stack

| Area | Tools |
|------|-------|
| Language | Python |
| Data handling | pandas, NumPy |
| Visualisation | Matplotlib, Seaborn, WordCloud |
| Machine learning | scikit-learn |
| NLP | NLTK, TF-IDF |
| Environment | Jupyter Notebook, VS Code, Git & GitHub |

---

## 🗂️ Repository Structure

```
OIBSIP/
├── README.md
├── DataScience-Task1-IrisClassification/
│   ├── Iris_Classification.ipynb
│   └── README.md
├── DataScience-Task4-SpamDetection/
│   ├── Spam_Detection.ipynb
│   ├── sms.tsv
│   └── README.md
└── DataScience-Task5-SalesPrediction/
    ├── Sales_Prediction.ipynb
    ├── Advertising.csv
    └── README.md
```

Each project folder has its own `README.md` with the approach, results and run instructions.

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/OIBSIP.git
cd OIBSIP

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn nltk wordcloud jupyter

# 3. Open any project's notebook
cd DataScience-Task1-IrisClassification
jupyter notebook Iris_Classification.ipynb
```

Datasets are included in the project folders (the Iris dataset ships with scikit-learn). NLTK stopwords download automatically on the first run of the spam notebook.

---

## 🧠 What I Learned

- Building a complete ML workflow rather than just fitting a model
- Choosing evaluation metrics that fit the problem (precision, recall and F1 for imbalanced data; MAE, RMSE and R² for regression)
- Preventing data leakage: fitting TF-IDF on training data only and removing duplicates before splitting
- Using cross-validation when the test set is small
- Reading model results carefully, such as interpreting coefficients versus feature importance
- Communicating findings in plain language with markdown explanations beside each chart

---

## 🎥 Demo Videos & LinkedIn Posts

| Project | Demo / LinkedIn Post |
|---------|---------------------|
| Iris Flower Classification | [Watch](#) |
| Spam Detection | [Watch](#) |
| Sales Prediction | [Watch](#) |

---

## 📬 Connect With Me

- 💼 LinkedIn: [Your LinkedIn URL]
- 🐙 GitHub: [Your GitHub URL]
- 📧 Email: [Your Email]

---

*Completed as part of the Oasis Infobyte Student Internship Program (OIBSIP) — Data Science track.*
#oasisinfobyte
