 📝 Review Sentiment Analysis
This project focuses on analyzing and classifying Amazon product reviews.
The goal is to preprocess the text data, extract meaningful features using NLP, and build machine learning models to predict review scores.

📚 Table of Contents
Project Overview
Dataset
Key Steps
Results
Insights
📘 Project Overview
This project analyzes user-written Amazon reviews using NLP and machine learning.
It involves text cleaning, feature extraction using TF-IDF, and model building for rating prediction (1–5).

📂 Dataset
The dataset consists of Amazon product reviews, with each entry containing:

ProductId: Product's unique ID
UserId: Reviewer’s ID
ProfileName: Reviewer’s name
HelpfulnessNumerator/Denominator: Helpfulness vote stats
Score: Rating (1 to 5)
Time: Review timestamp
ReviewSummary: Short summary
ReviewText: Full review content
📦 Sample file provided:

txt_reviews.zip: Sample raw review files
🔑 Key Steps
🔸 1. Data Extraction
Extract .txt reviews from ZIP
Load into a Pandas DataFrame
🔸 2. Preprocessing
Calculate helpfulness ratio
Convert Unix timestamp to datetime
Clean & tokenize reviews
Remove stopwords and lemmatize text
🔸 3. EDA (Exploratory Data Analysis)
Score distribution plots
Helpfulness rating visualizations
🔸 4. Text Vectorization
Apply TF-IDF to convert text into numerical vectors
🔸 5. Model Training
Trained and evaluated multiple classifiers:

Logistic Regression
Multinomial Naive Bayes
Gradient Boosting
Support Vector Machine (SVM)
Random Forest
📊 Results
Model	Accuracy
Logistic Regression	71.59% ✅
SVM	71.53%
Random Forest	70.23%
Gradient Boosting	67.55%
Multinomial Naive Bayes	65.74%
✅ Logistic Regression performed best among the models.

💡 Insights
Text data preprocessing significantly impacts model performance.
TF-IDF was effective for this task over raw tokens.
Logistic Regression and SVM gave close accuracy, but Logistic Regression had a slight edge.
Gradient Boosting underperformed possibly due to high feature dimensionality.
