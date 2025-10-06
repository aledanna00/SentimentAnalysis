
# 🎮 Sentiment Analysis on Videogame Reviews (Steam)

## 📌 Description

This project aims to perform **sentiment analysis** on videogame reviews from the **Steam** platform, using **NLP (Natural Language Processing)** techniques and **Text Classification** algorithms.

The goal is to automatically distinguish **positive** from **negative** reviews through an **ETL process**, machine learning models, and exploratory visualizations.

---

## 📂 Dataset

The dataset was obtained from Kaggle:
👉 [Steam Reviews & Games Dataset](https://www.kaggle.com/datasets/filipkin/steam-reviews)

It consists of two main files:

* **output_steamspy.csv** – Contains metadata about the games (ID, name, number of players).
* **output.csv** – Contains the reviews, labeled with `is_positive` (Positive/Negative).

---

## 🔧 Technologies and Libraries Used

* **Python**
* **Pandas, Numpy** → Data handling and manipulation
* **Re (RegEx)** → Text cleaning
* **Scikit-learn** → Machine learning models (Naive Bayes, Logistic Regression)
* **NLTK** → Natural language processing
* **Langdetect** → Language detection
* **Matplotlib, Seaborn** → Data visualization
* **WordCloud** → Textual representation

---

## 🛠️ Project Pipeline

1. **ETL (Extract, Transform, Load)**

   * Text cleaning and normalization (lowercasing, URL removal, symbols, spaces).
   * Language filtering (English-only reviews).
   * Class balancing (undersampling).

2. **Feature Extraction**

   * TF-IDF representation with n-grams up to trigrams.

3. **Classification Models**

   * **Naive Bayes (Multinomial)**
   * **Logistic Regression** (best model, with ≈ **91% accuracy**).

4. **Testing**

   * Evaluation on a synthetic dataset of positive and negative reviews.
   * Metrics: Accuracy, Precision, Recall, F1-score.

5. **Visualizations**

   * Word Clouds for positive and negative reviews.
   * Analysis of the **20 most distinctive words** for each class.

---

## 📊 Main Results

* **Logistic Regression** outperformed Naive Bayes in all major metrics.
* Overall accuracy ≈ **85%**.
* Good balance between **Precision** and **Recall**.
* Word Clouds highlight clear lexical differences between positive and negative reviews.

---

## 👨‍💻 Authors

* **Walter Di Sabatino**
* **Agnese Bruglia**
* **Alessandra D’Anna**

Polytechnic University of Marche – Academic Year 2024/2025