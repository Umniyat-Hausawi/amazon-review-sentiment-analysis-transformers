# 🗣️ Amazon Product Review Sentiment Analysis Using NLP & Machine Learning

An end-to-end Natural Language Processing (NLP) project for sentiment classification of Amazon customer reviews using both traditional Machine Learning techniques and Transformer-based models.

This project compares multiple approaches for text classification, starting from TF-IDF vectorization with classical machine learning models and ending with fine-tuned DistilBERT for sentiment prediction.

---

## 📌 Project Overview

Customer reviews are one of the most valuable sources of feedback for e-commerce businesses. However, manually reading thousands of reviews is inefficient and not scalable.

This project aims to automatically classify Amazon customer reviews into:

- **Positive**
- **Neutral**
- **Negative**

By transforming raw review text into meaningful numerical representations and training multiple classification models.

---

## 🎯 Business Problem

E-commerce companies receive massive volumes of customer feedback daily.

Without automated sentiment analysis, businesses may struggle to:

- Identify dissatisfied customers quickly
- Detect product issues
- Understand customer satisfaction trends
- Monitor mixed or neutral feedback

The challenge addressed in this project:

> Can we build a machine learning model that automatically classifies customer sentiment from review text?

---

## 📂 Dataset

**Dataset Source (Kaggle):**  
[Amazon Product Reviews Dataset](https://www.kaggle.com/datasets/arhamrumi/amazon-product-reviews?utm_source=chatgpt.com)

The dataset contains Amazon customer reviews and ratings, which were transformed into sentiment categories for supervised text classification.

### Sentiment Label Mapping

| Rating | Sentiment |
|--------|------------|
| 1–2 | Negative |
| 3 | Neutral |
| 4–5 | Positive |

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLP (Natural Language Processing)
- TF-IDF Vectorization
- Transformers (Hugging Face)
- DistilBERT

---

## ⚙️ Machine Learning Pipeline

The project follows a complete NLP workflow:

### 1. Business Problem Definition
Understanding the real-world business use case and defining the sentiment classification objective.

### 2. Dataset Loading & Understanding
Loading the Amazon review dataset and exploring its structure.

### 3. Sentiment Label Creation
Converting numerical ratings into sentiment classes:

- Negative
- Neutral
- Positive

### 4. Exploratory Data Analysis (EDA)
Analyzing:

- Review distribution
- Sentiment balance
- Review lengths
- Data quality

### 5. Text Preprocessing
Cleaning text data by:

- Lowercasing
- Removing unnecessary symbols
- Text normalization

### 6. Feature Engineering

#### Traditional NLP Approach
- TF-IDF Vectorization
- TF-IDF + Bigrams

#### Transformer-Based Approach
- Tokenization using DistilBERT tokenizer
- Sequence length optimization
- Padding & truncation

### 7. Train/Test Split
Splitting the dataset into training and testing sets for fair evaluation.

### 8. Model Training

Several models were trained and compared:

#### Traditional Machine Learning Models
- Logistic Regression + TF-IDF
- Logistic Regression + TF-IDF + Bigrams
- Linear SVM + TF-IDF + Bigrams

#### Transformer Model
- DistilBERT Fine-Tuning

### 9. Model Evaluation

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Error Analysis

---

## 📊 Model Performance Comparison

| Model | Accuracy |
|--------|------------|
| DistilBERT Fine-Tuning | **75.35%** |
| Logistic Regression + TF-IDF + Bigrams | 71.17% |
| Linear SVM + TF-IDF + Bigrams | 70.53% |
| Logistic Regression + TF-IDF | 69.67% |

### Key Observation

The Transformer-based model (**DistilBERT**) achieved the highest performance, outperforming traditional machine learning approaches.

---

## 🔍 Error Analysis & Insights

The model performed best on:

✅ **Positive Reviews**

The biggest challenge remained:

⚠️ **Neutral Reviews**

Neutral sentiment showed lower performance because neutral feedback often overlaps semantically with both positive and negative opinions, making classification more ambiguous.

This reflects a realistic NLP challenge in sentiment analysis.

---

## 📈 Key Findings

- Transformer models outperform traditional TF-IDF approaches in contextual understanding.
- Positive sentiment is easier to classify due to stronger emotional signals.
- Neutral reviews remain difficult because of ambiguity and mixed wording.
- Feature engineering such as **bigrams** improved traditional model performance.

---

## 🚀 Future Improvements

Potential next steps include:

- Experimenting with larger transformer models
- Binary sentiment classification (Positive vs Negative)
- Hyperparameter tuning
- Handling class ambiguity more effectively
- Deploying the model as an API or web application

---

## 🧠 Conclusion

This project demonstrates a complete NLP workflow for sentiment classification using both traditional machine learning and transformer-based architectures.

Through experimentation and comparison, **DistilBERT Fine-Tuning achieved the best performance with 75.35% accuracy**, showing stronger contextual understanding than TF-IDF-based models.

The project also highlights a realistic NLP challenge: **neutral sentiment classification remains difficult due to ambiguity and overlap between sentiment classes**.

Overall, this project demonstrates practical experience in:

- NLP preprocessing
- Feature engineering
- Machine learning model comparison
- Transformer fine-tuning
- Model evaluation and interpretation
- Translating technical outputs into business insights

---

## 👤 Author

**Umniyat Hausawi**  
Aspiring Data Scientist | AI & NLP Projects
