# 📰 Fake News Prediction using Machine Learning

## 📌 Overview
Detecting fake news is an important challenge in the digital age.  
This project applies **Machine Learning** and **Natural Language Processing (NLP)** techniques to automatically classify news stories as **real or fake**.  

It uses the **WELFake Dataset (70,000+ news items)**, which includes both headlines and article texts.  
The workflow covers extensive preprocessing and multiple classification models.

---

## 📊 Dataset Details
- **Source:** [WELFake Dataset (Kaggle)](https://www.kaggle.com/)  
- **Size:** 70,000+ news samples  

**Features:**
- `title`: The headline of the article  
- `text`: Full news story  
- `label`: `0 = Real news`, `1 = Fake news`

---

## 🔄 Workflow & Model Details

### 🧹 Preprocessing
- **Tokenization** → Splitting text into words  
- **Stopword Removal** → Eliminating common words (e.g., *the, is, a*)  
- **Stemming** → Reducing words to their root forms  
- **Library Used:** [NLTK](https://www.nltk.org/)  

### ✨ Feature Extraction
- **TF-IDF Vectorization** (Term Frequency–Inverse Document Frequency)  
- Converts cleaned text into numerical features for ML models  

### 🤖 Model Training
Several machine learning models are trained and compared:
- **Logistic Regression** → Simple, robust baseline  
- **Random Forest** → Ensemble model, high accuracy  
- **Decision Tree** → Fast, interpretable  
- **Support Vector Classifier (SVC)** → Strong for text classification  

### 📈 Evaluation Metrics
- **Accuracy Score**  
- **Confusion Matrix**  
- **Classification Report** → *Precision, Recall, F1-Score*  

---

## 🚀 Quick Start

### 1️⃣ Install dependencies
```bash
pip install -r requirements.txt
```
### 2️⃣ Download the dataset
Download the **WELFake Dataset** from Kaggle and place it inside an `input/` folder.

### 3️⃣ Run the notebook
```bash
jupyter notebook fake-news-detection.ipynb
```

## 🏆 Results
- Models achieve **85–93% accuracy** (depending on the model)  
- **Random Forest** and **SVC** often outperform simpler models  
- All metrics and confusion matrices are available in the notebook  

---

## 🔮 Future Plans
- Implement advanced models: **LSTM, BERT** for deeper language understanding  
- Add **model interpretation tools** (e.g., SHAP, LIME)  
- Package as a **web app** for real-time fake news detection  

---

## 👨‍💻 Author
Created by an **AI/ML & MLOps enthusiast**, currently a **final-year student in India**, preparing for higher education exams and developing practical ML projects.  

---

## 📜 License
Open for **educational and research purposes**.  
Recommended: [MIT License](https://opensource.org/licenses/MIT)  

---
