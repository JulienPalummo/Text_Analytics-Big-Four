# Big 4 Employee Sentiment and Career Insights  

This repository contains a comprehensive analysis of employee reviews from the Big 4 accounting firms.  
The project integrates Natural Language Processing (NLP), machine learning, and recommendation techniques to:  

1. Analyze textual employee feedback for sentiment and thematic trends.  
2. Predict employee ratings from unstructured review data.  
3. Extract dominant career-related topics using topic modeling.  
4. Provide career recommendations to potential candidates based on textual and numerical patterns.  

By combining quantitative modeling with qualitative insights, this project highlights how employee perceptions vary across the Big 4 and how such data can inform both job seekers and HR decision-making.  

---

## 📂 Project Structure  

- **4 - combined_code OFFICIAL.py** → End-to-end pipeline: preprocessing, sentiment scoring, regression, topic modeling, recommender system.  
- **df_big4.csv** → Dataset of employee reviews with firm name, job role, rating, and free-text feedback.  
- **Final_Project.pdf** → Project report documenting methodology, results, and interpretations.  

---

## ⚙️ Features and Workflow  

### 1. Data Preprocessing  
- Standardized review dataset with firm, role, rating, and free-text fields.  
- Applied text cleaning: lowercasing, punctuation removal, stopword filtering, lemmatization.  
- Constructed structured features (e.g., average rating per firm, review length, sentiment scores).  

### 2. Sentiment Analysis  
- **VADER** and **TextBlob** applied to capture polarity and subjectivity.  
- Sentiment scores correlated with numerical employee ratings, validating their predictive power.  

### 3. Regression Modeling  
- Goal: predict review ratings from sentiment and other features.  
- Models tested:  
  - Linear Regression  
  - Random Forest  
  - Gradient Boosting  
- Gradient Boosting achieved the best performance, showing that review text carries strong predictive signals about satisfaction.  

### 4. Topic Modeling (LDA)  
- Extracted recurring themes in reviews to capture qualitative aspects of employee experience.  
- Key topics across firms included:  
  - Work-life balance and long hours  
  - Career advancement and promotion opportunities  
  - Compensation and benefits  
  - Management support and culture  
- Comparative topic prevalence highlighted differences between firms.  

### 5. Recommendation System  
- Built a **content-based recommender** leveraging similarity in sentiment and role descriptions.  
- Allows job seekers to receive suggestions on which firm aligns most with their preferences.  

---

## 📈 Results & Key Findings  

- **Sentiment → Ratings Link:** Sentiment polarity is a reliable predictor of employee satisfaction.  
- **Firm-Level Differences:** While all firms share common themes (e.g., long hours), some emphasize **career growth**, others focus on **team culture** or **pay/benefits**.  
- **Predictive Modeling:** Gradient Boosting captured non-linear relationships and outperformed baseline models.  
- **Topic Modeling:** Clear, interpretable themes emerged, confirming the qualitative richness of employee feedback.  
- **Recommendations:** A personalized recommendation layer adds practical value for prospective employees.  

---

## 🛠️ Tech Stack  

- **Language:** Python  
- **Libraries:** pandas, scikit-learn, nltk, gensim, seaborn, matplotlib, TextBlob, VADER  
- **Techniques:** Sentiment Analysis, Regression, Topic Modeling (LDA), Recommendation Systems  
