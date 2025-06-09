# Fintech Reviews Analytics

This project is part of the 10 Academy Week 2 Challenge. The goal is to analyze user reviews from the Google Play Store for three Ethiopian banking apps and provide data-driven insights to improve customer experience.

---

## 📌 Task 1: Data Collection and Preprocessing

**Objective:**  
Scrape, clean, and structure user reviews for three banking apps:
- Dashen Bank
- Commercial Bank of Ethiopia (CBE)
- Bank of Abyssinia (BOA)

**Steps Completed:**
- Scraped 500 reviews per bank using `google-play-scraper`.
- Collected review text, rating, date, bank name, and source.
- Removed duplicates and rows with missing values.
- Saved cleaned dataset to `data/cleaned_reviews_<timestamp>.csv`.

---

## 📊 Task 2: Sentiment Analysis (In Progress)

**Objective:**  
Classify reviews into positive, neutral, or negative sentiment using VADER sentiment analysis.

**Steps Completed:**
- Loaded cleaned data from Task 1.
- Applied sentiment analysis using VADER (rule-based sentiment scoring).
- Added `sentiment` column to the dataset.
- Grouped reviews by bank and sentiment for further analysis.

**Next Steps:**
- Visualize sentiment trends.
- Extract and group review themes using keyword techniques (e.g., TF-IDF or spaCy).

---

## 📁 Project Structure

fintech-reviews-analytics/
├── data/ # Cleaned review datasets
├── notebooks/
│ └── task1_scraping.ipynb # Scraping and sentiment analysis
├── README.md
├── requirements.txt
└── .gitignore

yaml
Copy
Edit

---

## 🚀 Technologies Used

- Python
- Pandas
- Google Play Scraper
- VADER Sentiment Analyzer
- Jupyter Notebook
