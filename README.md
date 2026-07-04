# 🛍️ Amazon Footwear EDA — Data Pipeline & Analysis

An end-to-end data project that scrapes, cleans, and analyzes real Amazon footwear listings to uncover what actually drives sales in the category — brand strength, pricing sweet spots, ratings, and demographic focus — and turns those findings into concrete recommendations for sellers.

---

## 📌 Problem Statement

Amazon doesn't expose a structured, analysis-ready view of footwear product performance — just raw, unstructured listings spread across search result pages. This project builds a pipeline to turn that raw data into a clean dataset and answers a practical question sellers actually care about:

> **Which brands, price points, and product attributes drive the most footwear sales on Amazon — and what should a seller do differently?**

---

## 🛠️ Tech Stack

| Stage | Tools |
|---|---|
| Extraction | Python, BeautifulSoup, Requests |
| Transformation & Cleaning | Pandas, NumPy |
| Analysis | Pandas, Descriptive Statistics |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## 🔄 Approach (Pipeline Overview)

1. **Extract** — Scraped 900+ Amazon footwear product listings using BeautifulSoup, pulling 11 key features per product (brand, price, rating, category, gender focus, water resistance, discount %, etc.).
2. **Transform** — Cleaned the raw scraped data: handled missing values, standardized inconsistent price/rating formats, removed duplicates, and normalized category labels.
3. **Load** — Structured the cleaned output into a single analysis-ready dataset (CSV).
4. **Analyze** — Ran exploratory data analysis to surface brand-level, pricing, and demographic patterns.
5. **Report** — Translated findings into a plain-language strategy summary for sellers and marketers.

---

## 🔍 Key Insights

- **Top brands**: Bata, Sparx, and Doctor Extra Soft together account for **60%+** of total footwear sales.
- **Category mix**: Sandals, slippers, and shoes make up **80%** of category sales volume.
- **Ratings matter**: Products rated **≥ 4.0** achieved **30–40% more sales** than lower-rated listings.
- **Pricing sweet spot**: Moderately priced items (**₹400–₹700**) showed the highest conversion; extreme discounts had minimal impact.
- **Demographics**: Female-focused footwear drove **54%** of total sales, while unisex products underperformed.
- **Water resistance**: Affected only **4.4%** of purchases — a low-priority feature for inventory planning.

---

## 📁 Repository Structure

```
amazon-footwear-eda/
├── data/
│   ├── raw/                # Scraped, unprocessed listings
│   └── processed/          # Cleaned, analysis-ready dataset
├── notebooks/
│   ├── 01_scraping.ipynb       # Extraction logic (BeautifulSoup)
│   ├── 02_cleaning.ipynb       # Data cleaning & transformation
│   └── 03_eda_analysis.ipynb   # EDA, visualizations, insights
├── reports/
│   └── strategy_report.md      # Seller-facing recommendations
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

```bash
git clone https://github.com/gunavardhanrao/amazon-footwear-eda.git
cd amazon-footwear-eda
pip install -r requirements.txt
jupyter notebook notebooks/03_eda_analysis.ipynb
```

---

## 💡 Key Learnings

- Roughly 70–80% of the effort in a real pipeline goes into cleaning and validation, not the analysis itself — raw scraped data is rarely usable as-is.
- Designing a consistent schema up front (11 well-defined features) made downstream analysis and visualization far faster.
- Translating statistical findings into plain, actionable recommendations is as important as the analysis for a non-technical audience (sellers/marketers).

---

## 📊 Sample Visualization

<img width="1287" height="911" alt="image" src="https://github.com/user-attachments/assets/d03c171b-5930-4f90-a508-b39a699ea79e" />

---

## 🙋 Author

**Appaji Gunavardhan Rao**
📧 gunavardhanrao8@gmail.com | [LinkedIn](https://linkedin.com/in/appaji-gunavardhan-rao) | [GitHub](https://github.com/gunavardhanrao)
