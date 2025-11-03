# 🏛️ Web Scraping & NLP Analysis of Architectural Styles

A Python project that scrapes Wikipedia to collect and analyze architectural styles using text mining and NLP techniques. This pipeline turns raw articles into structured data and visual insights.

## What It Does

- Scrapes Wikipedia: Extracts titles, URLs, and full text of articles on architectural styles

- Text Processing & NLP: Uses TF-IDF and other NLP methods to explore linguistic and thematic similarities

- Automated & Reproducible: Logging, retries, Parquet storage, and workflow orchestration with Prefect

- Visualizations: Generates plots with Matplotlib and Seaborn to highlight patterns and insights

## Tech & Tools

Python

pandas, BeautifulSoup, requests, tqdm

NLP: TF-IDF, NLTK, wordcloud

Data validation & testing: pandera, pytest

Visualization: matplotlib, seaborn

Workflow orchestration: Prefect

## How to Run

Clone the repository:

git clone https://github.com/AnissaKerouaz/Web-Scraping-and-NLP-Analysis-of-Architectural-Styles.git
cd architectural-styles-nlp


Install dependencies:

pip install -r requirements.txt


Run the scraper and metadata fetcher:

python titles_urls.py   # Scrape article titles and URLs
python text_metadata.py # Fetch full text and categories


Visualizations and processed data will be available in the data/ and visualizations/ folders.

## Notes

The scraper includes polite delays and retries to avoid overloading Wikipedia servers.

Configurations for start URL, headers, and output paths can be updated in config.py.
