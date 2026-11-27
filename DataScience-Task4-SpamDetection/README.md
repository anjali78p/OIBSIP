# Spam Detection with Machine Learning

**Oasis Infobyte SIP — Data Science, Task 4**

An NLP classifier that separates spam from ham (legitimate) messages.

## Files
- `Spam_Detection.ipynb` — full notebook
- `sms.tsv` — SMS Spam Collection dataset (label, message)

## Approach
1. Load data, check class distribution (about 87% ham / 13% spam, so imbalanced)
2. Text preprocessing: lowercase, punctuation removal, stopword removal (NLTK), stemming (Porter)
3. Remove exact duplicate messages before splitting
4. TF-IDF features (unigrams and bigrams, top 5000)
5. 80/20 stratified split
6. Models: Multinomial Naive Bayes, Logistic Regression, Linear SVM
7. Metrics: accuracy, precision, recall, F1, confusion matrix
8. Discussion of why recall matters for spam detection, and word clouds for spam vs ham

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Linear SVM | 0.978 | 0.915 | 0.908 | 0.912 |
| Multinomial Naive Bayes | 0.975 | 0.949 | 0.847 | 0.895 |
| Logistic Regression | 0.969 | 0.861 | 0.901 | 0.881 |

**Best model:** Linear SVM (highest F1).

## Run it
```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk wordcloud jupyter
jupyter notebook Spam_Detection.ipynb
```
Keep `sms.tsv` in the same folder as the notebook. NLTK stopwords download automatically on the first run.
