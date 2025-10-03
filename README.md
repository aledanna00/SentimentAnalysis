# 🎮 Sentiment Analysis su Recensioni di Videogiochi (Steam)

## 📌 Descrizione

Questo progetto ha come obiettivo l’analisi del sentiment delle recensioni di videogiochi provenienti dalla piattaforma **Steam**, utilizzando tecniche di **NLP (Natural Language Processing)** e algoritmi di **Text Classification**.

L’idea è quella di distinguere automaticamente recensioni **positive** da recensioni **negative**, applicando un processo di **ETL**, modelli di machine learning e visualizzazioni esplorative.

## 📂 Dataset

Il dataset è stato reperito da Kaggle:
👉 [Steam Reviews & Games Dataset](https://www.kaggle.com/datasets/filipkin/steam-reviews)

È composto da due file principali:

* **output_steamspy.csv**: contiene metadati sui videogiochi (ID, nome, numero di giocatori).
* **output.csv**: contiene le recensioni, con etichetta `is_positive` (Positive/Negative).

## 🔧 Tecnologie e Librerie Utilizzate

* **Python**
* **Pandas, Numpy** → gestione e manipolazione dati
* **Re (RegEx)** → pulizia testo
* **Scikit-learn** → modelli di machine learning (Naive Bayes, Logistic Regression)
* **NLTK** → elaborazione del linguaggio naturale
* **Langdetect** → rilevamento lingua
* **Matplotlib, Seaborn** → visualizzazioni
* **WordCloud** → rappresentazioni testuali

## 🛠️ Pipeline del Progetto

1. **ETL (Extract, Transform, Load)**

   * Pulizia e normalizzazione del testo (minuscole, rimozione URL, simboli, spazi).
   * Filtraggio linguistico (solo recensioni in inglese).
   * Bilanciamento delle classi (undersampling).

2. **Feature Extraction**

   * Rappresentazione TF-IDF con n-grammi fino a trigrams.

3. **Modelli di Classificazione**

   * **Naive Bayes (Multinomial)**
   * **Logistic Regression** (miglior modello, con accuratezza ≈ **91%**).

4. **Testing**

   * Valutazione con dataset sintetico di recensioni positive/negative.
   * Metriche: Accuracy, Precision, Recall, F1-score.

5. **Visualizzazioni**

   * Word Cloud per recensioni positive e negative.
   * Analisi delle **20 parole più distintive** per ciascuna classe.

## 📊 Risultati Principali

* **Logistic Regression** ha superato il Naive Bayes in tutte le metriche principali.
* Accuratezza complessiva ≈ **91%**.
* Buon equilibrio tra **Precision** e **Recall**.
* Word Cloud evidenzia differenze lessicali tra recensioni positive e negative.

## 👨‍💻 Autori

* **Walter Di Sabatino**
* **Agnese Bruglia**
* **Alessandra D’Anna**

Università Politecnica delle Marche – A.A. 2024/2025

---

Vuoi che ti prepari anche un file `requirements.txt` con tutte le librerie principali già elencate?
