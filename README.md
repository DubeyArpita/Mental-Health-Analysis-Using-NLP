# Mental-Health-Analysis-Using-NLP

This repository contains code for a machine learning project that classifies text messages to identify potential mental health issues. The project uses various NLP techniques and models to predict whether a given text is associated with mental health struggles (`label 1`) or not (`label 0`).

---

## 🎯 Aim

The main objective is to **classify if a person is struggling with mental health issues** from their text messages. This is a critical step toward providing timely support and intervention.

---

## 💾 Dataset

The model is trained on the `mental_health.csv` dataset, which includes two columns:

* `text`: The text content of the message.
* `label`: The corresponding label (1 for mental health-related, 0 for not).

This dataset is valuable for researchers and professionals interested in understanding the language and sentiment surrounding mental health.

---

## 🛠️ Dependencies

To run the code, you'll need the following Python libraries:

* **pandas**
* **numpy**
* **matplotlib**
* **wordcloud**
* **nltk**
* **sklearn**

You can install these dependencies using `pip`:

```bash
pip install pandas numpy matplotlib wordcloud nltk scikit-learn
```
# Method

The project follows a standard machine learning pipeline:

1.  **Data Loading and Preprocessing**: The `mental_health.csv` file is loaded. Text data is cleaned by removing punctuation, converting to lowercase, and handling stop words.

2.  **Feature Extraction**: The preprocessed text is converted into numerical features that machine learning models can understand. Techniques like **TF-IDF (Term Frequency-Inverse Document Frequency)** are used for this step.

3.  **Model Training**: Several machine learning classifiers (e.g., **Logistic Regression**, **Naive Bayes**) are trained on the preprocessed data and extracted features.

4.  **Evaluation**: The trained models are evaluated on a separate test set to measure their accuracy and performance.

This methodology combines NLP with machine learning to build an automated system for identifying signals of mental distress in text.
