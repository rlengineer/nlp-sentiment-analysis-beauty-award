# NLP Sentiment Analysis of Beauty Awards

## Overview
This project analyzes whether customer sentiment and review language can distinguish — and predict — *Allure Best of Beauty 2024* award winners using large-scale Sephora customer review data. By combining natural language processing (NLP), sentiment analysis, and machine learning, the study explores how consumer perception aligns with industry-recognized excellence in the beauty space.

The project leverages over **778,000 customer reviews** across **7,000+ products**, including **85 Best of Beauty 2024 award winners**, to evaluate sentiment differences, keyword signals, and predictive modeling performance.

---

## Research Questions
1. How does customer sentiment differ between *Best of Beauty* award winners and non-award-winning products?
2. Using customer ratings and sentiment scores, how accurately can we predict whether a product will be a *Best of Beauty* winner?
3. Are there specific keywords in customer reviews that distinguish award winners from non-winners, and can these keywords help predict future award recipients?

---

## Data
- **Source:** Sephora customer reviews
- **Collection Method:** Web scraping
- **Scale:**
  - 778,000+ customer reviews  
  - 7,000+ beauty products  
  - 85 Allure *Best of Beauty 2024* award winners

Raw review data is **not included** in this repository due to size and source restrictions.  
A small processed sample dataset is provided for demonstration and reproducibility purposes.

---

## Methodology

### Exploratory Data Analysis (EDA)
- Compared rating distributions, review volume, and sentiment scores between award winners and non-winners
- Visualized key differences using bar charts and distribution plots

### Text Processing & Feature Engineering
- Cleaned and tokenized review text
- Applied **TF-IDF** to identify distinguishing keywords
- Used **VADER sentiment analysis** to compute sentiment scores for each product

### Modeling
Several classification models were trained to predict award status:
- Logistic Regression
- Random Forest
- XGBoost

Models were evaluated using classification accuracy and comparative performance across feature sets.

---

## Results
- Award-winning products tend to exhibit higher average sentiment scores and ratings
- Certain review keywords are disproportionately associated with award winners
- Classification models demonstrate that customer sentiment and ratings provide meaningful predictive signal for award outcomes

(See `/figures` and `/reports` for detailed visualizations and results.)

---

## Repository Structure

```text
nlp-sentiment-analysis-beauty-awards/
├── reports/          # Academic paper and presentation
├── figures/          # EDA and modeling visualizations (PNG)
├── src/              # Python source code (EDA, NLP, models)
├── notebooks/        # Exploratory and modeling notebooks
├── data/             # Sample processed data + documentation
├── config/           # Configuration templates (no credentials)
└── scripts/          # Pipeline and utility scripts
