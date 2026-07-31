## ReviewSense | NLP-Based Amazon Review Rating Prediction

A Machine Learning and Natural Language Processing (NLP) project that analyzes Amazon product reviews and predicts review ratings (1–5 stars) based on textual content. The project applies text preprocessing, TF-IDF feature extraction, and multiple classification algorithms to evaluate sentiment prediction performance.

---

## 📖 Project Overview

This project focuses on analyzing user-written Amazon product reviews using **Natural Language Processing (NLP)** and **Machine Learning** techniques. The workflow includes data preprocessing, feature engineering, exploratory data analysis, and model training to classify review scores accurately.

---

## 📂 Dataset

The dataset contains Amazon product reviews with the following attributes:

| Feature | Description |
|---------|-------------|
| **ProductId** | Unique product identifier |
| **UserId** | Reviewer identifier |
| **ProfileName** | Reviewer's name |
| **HelpfulnessNumerator** | Helpful votes received |
| **HelpfulnessDenominator** | Total helpfulness votes |
| **Score** | Product rating (1–5) |
| **Time** | Review timestamp |
| **ReviewSummary** | Short review summary |
| **ReviewText** | Complete review text |

### 📦 Sample Data

- `txt_reviews.zip` – Sample raw Amazon review files

---

## 🚀 Project Workflow

### 1️⃣ Data Extraction
- Extract review files from ZIP archive
- Load reviews into a Pandas DataFrame

### 2️⃣ Data Preprocessing
- Calculate helpfulness ratio
- Convert Unix timestamps into readable dates
- Clean review text
- Tokenize sentences
- Remove stopwords
- Perform lemmatization

### 3️⃣ Exploratory Data Analysis (EDA)
- Rating distribution analysis
- Helpfulness score visualization
- Review length analysis
- Statistical summaries

### 4️⃣ Feature Engineering
- Convert textual reviews into numerical vectors using **TF-IDF Vectorization**

### 5️⃣ Model Training
The following Machine Learning models were trained and evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting
- Multinomial Naive Bayes

---

## 📊 Model Performance

| Model | Accuracy |
|--------|----------|
| ✅ Logistic Regression | **71.59%** |
| Support Vector Machine (SVM) | **71.53%** |
| Random Forest | **70.23%** |
| Gradient Boosting | **67.55%** |
| Multinomial Naive Bayes | **65.74%** |

🏆 **Best Performing Model:** Logistic Regression

---

## 💡 Key Insights

- Proper text preprocessing significantly improves prediction accuracy.
- TF-IDF feature extraction performs effectively for sentiment classification.
- Logistic Regression achieved the highest accuracy among all evaluated models.
- SVM delivered comparable performance with only a marginal difference.
- Random Forest provided competitive results but slightly lower accuracy.
- Gradient Boosting struggled with the high-dimensional sparse feature space.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📈 Future Improvements

- Deep Learning models (LSTM, Bi-LSTM)
- Transformer-based models (BERT, RoBERTa)
- Hyperparameter tuning
- Class imbalance handling
- Deployment using Streamlit or Flask

---

## 📌 Conclusion

This project demonstrates how **Natural Language Processing (NLP)** and **Machine Learning** can be combined to analyze customer reviews and predict product ratings effectively. Among all evaluated models, **Logistic Regression** achieved the highest accuracy, making it the most suitable baseline model for this dataset.
