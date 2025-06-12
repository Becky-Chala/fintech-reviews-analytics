# Fintech Customer Review Analysis

This project is part of the 10 Academy Week 2 Challenge. It focuses on collecting, analyzing, and storing customer reviews from Ethiopian banking apps to extract insights using sentiment and thematic analysis.

---

## 📦 Project Structure

```
fintech-reviews-analytics/
├── data/                        # Cleaned review datasets
├── notebooks/
│   └── task1_scraping.ipynb     # Full workflow from Task 1–4
├── .venv/                       # Python virtual environment (not pushed)
├── requirements.txt             # Project dependencies
└── README.md                    # Project overview and instructions
```

---

## 🔍 Overview of Tasks

### ✅ Task 1: Scrape Customer Reviews
- Scraped reviews using `google_play_scraper` for:
  - Dashen Bank
  - Commercial Bank of Ethiopia (CBE)
  - Bank of Abyssinia (BOA)
- Cleaned and saved reviews to a CSV file in the `/data` folder.

### ✅ Task 2: Sentiment & Theme Analysis
- Applied **VADER sentiment analysis** to classify each review as Positive, Neutral, or Negative.
- Extracted simple **themes** based on keyword matching.
- Visualized sentiment distribution by bank.

### ✅ Task 3: Store Data in Oracle
- Installed and connected to Oracle XE locally.
- Created a `REVIEWS` table with fields like rating, sentiment, themes, and bank name.
- Inserted all cleaned and annotated review data into Oracle.

### ✅ Task 4: Query & Analyze Data
- Queried the `REVIEWS` table into pandas.
- Performed analytical summaries:
  - Sentiment breakdown by bank
  - Monthly review volume trends
  - Top mentioned themes
  - Average rating per bank
- Used `matplotlib` and `seaborn` for visualizations.

---

## 💻 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/Becky-Chala/fintech-reviews-analytics.git
   cd fintech-reviews-analytics
   ```
2. Set up a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open the notebook:
   ```bash
   jupyter notebook notebooks/task1_scraping.ipynb
   ```

Make sure Oracle Instant Client is installed and configured if running Task 3 or 4.

---

## 📚 Dependencies

- `google_play_scraper`
- `pandas`
- `matplotlib`
- `seaborn`
- `nltk` (for VADER)
- `cx_Oracle`

---

## 📈 Output

- Cleaned reviews with sentiment and themes in `/data`
- Oracle database with full `REVIEWS` table
- Visual insights showing customer feedback trends
