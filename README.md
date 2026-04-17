# trainer-quotes-analysis
# 💪 Trainer Quotes — Data Pipeline & Analysis

A Python data pipeline that automatically collects, filters, and analyses inspirational quotes tailored specifically for trainers and coaches. Built in Jupyter Notebook using a rule-based classification algorithm.

---

## What it does

This project scrapes quotes from a website, runs them through a custom-built classifier to keep only quotes relevant to **empowerment, learning, and growth**, and produces a series of visualisations to analyse the results.

The end output is a curated, ready-to-use quotes dataset exported as CSV — including a shortlist of punchy quotes under 15 words, ideal for social media captions, client check-ins, or session openers.

---

## How it works

The pipeline follows a classic **ETL pattern**:

- **Extract** — collects quotes automatically across all pages of the source website using `requests` and `BeautifulSoup`
- **Transform** — passes each quote through a rule-based binary classifier that checks for relevant tags, empowerment keywords, and filters out anything too generic
- **Load** — exports the filtered, analysis-ready dataset to CSV

The classifier is **deterministic** — every decision is traceable back to an explicit rule, making it fully transparent and easy to adjust.

---

## Visualisations

- Most represented authors in the collection
- Most common themes and tags
- Quote length distribution (short vs medium vs long)
- Top 20 power words used across all quotes

---

## Output files

| File | Description |
|------|-------------|
| `trainer_quotes.csv` | Full filtered quote collection |
| `trainer_quotes_social.csv` | Shortlist of quotes under 15 words |

---

## Tech stack

| Library | Purpose |
|---------|---------|
| `requests` | Fetching web pages |
| `BeautifulSoup` | Parsing HTML |
| `pandas` | Data cleaning and analysis |
| `matplotlib` | Visualisations |
| `seaborn` | Chart styling |

---

## Skills demonstrated

- Web scraping with automatic pagination
- Rule-based classification algorithm (deterministic binary classifier)
- ETL pipeline design
- Exploratory Data Analysis (EDA)
- Text analysis and word frequency (NLP fundamentals)
- Data visualisation

---

## How to run

1. Clone the repository
2. Open `trainer_quotes_scraper.ipynb` in Jupyter Notebook or Google Colab
3. Run all cells from top to bottom (**Kernel → Restart & Run All**)
4. CSV files and chart images will be saved automatically

---

## Author

Built as part of a Python data skills development project.
