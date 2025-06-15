# # 📰 Fake News Detector (LSTM + BERT)

This project focuses on analyzing fake and real news articles using Natural Language Processing (NLP) techniques. The dataset contains labeled news data, and our goal in this stage is to extract insights, visualize patterns, and prepare for future machine learning classification.

---

## 📂 Dataset

**Source**: [Kaggle Fake News Dataset](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets)
The dataset consists of news articles with the following features:
- `title`
- `text`
- `label` (0 for fake, 1 for real)

---

## 🧠 Model Details

### 🔸 LSTM Model

- Pre-trained GloVe word embeddings (`glove.6B.100d.txt`)
- Bidirectional LSTM to capture contextual flow from both directions
- Dense layers with dropout for regularization
- Sigmoid activation for binary classification

### 🔸 BERT Model

- Tokenization using `bert-base-uncased`
- Deep contextual understanding through attention mechanism
- Fine-tuned end-to-end using HuggingFace `Transformers`
- Higher performance for nuanced linguistic detection

---


## 🧹 Data Cleaning & Preprocessing

- Converted all text to lowercase
- Removed stop words, punctuation, and special characters
- Tokenized and cleaned the corpus using NLP techniques

---

## 📊 Exploratory Data Analysis

### ✅ Word Cloud
- Generated separate word clouds for **fake** and **real** news
- Helped visualize the most frequent words in each category

### ✅ Top 20 Words Bar Chart
- Bar plots showing the top 20 most used words in **fake news** and **real news**
- Identified commonly used terms and themes in each class

### ✅ Article Length Distribution
- Histogram of article lengths
- Found that **real news articles tend to be longer** than fake ones

### ✅ Document-Term Matrix (DTM)
- Constructed a sparse matrix representation of word frequencies across articles
- Prepared the foundation for vectorization and future model training

---

## 📌 Key Insights

- Fake news articles often contain emotionally charged or sensational words.
- Real news articles are more formal and longer in length.
- There is a noticeable difference in vocabulary usage between real and fake articles.

---

## ✅ Conclusion

The exploratory data analysis reveals distinct textual patterns between fake and real news articles. These patterns serve as a strong base for building classification models. The insights gained from the word clouds, term frequencies, and text length distributions provide valuable direction for model selection and feature engineering in the next phase of the project.

---

## 🚧 Next Steps

- Apply **TF-IDF Vectorization**
- Train models like **BERT**, **LSTM**.
- Evaluate performance using metrics like **accuracy**, **precision**, and **recall**

---

## 🔧 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn
- `tm` and `wordcloud` (R)
- scikit-learn (planned for model phase)

---

## 👨‍💻 Author

**Achuth Akilesh**  
*Data Analyst & UI/UX Enthusiast*







