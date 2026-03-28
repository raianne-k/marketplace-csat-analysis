# marketplace-csat-analysis
Marketplace CSAT review ( Olist / Kaggle )

**Domain:** B2C Marketplace / Retail  
**Tools:** Python, Pandas, Plotly  
**Dataset:** [Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (Kaggle, CC BY-NC-SA 4.0)  
**Notebook:** [View on Kaggle](https://www.kaggle.com/code/raiannekuzer/marketplace-csat-analysis)

---

## Business Context

This project investigates what drives customer satisfaction in a marketplace environment, with a focus on delivery performance and seller variation.

The core question was simple: if customer satisfaction is falling, what is actually driving the bad experiences?

The analysis follows the Google Data Analytics six-phase framework: Ask, Prepare, Process, Analyze, Share, and Act.

---

## Guiding Questions (ASK)

1. What drives satisfaction in customer satisfaction?
2. How does delivery performance impact CSAT?
3. Is seller performance a key mechanism behind issues?

---

## Key Findings

| # | Finding | Key Stat |
|---|---------|----------|
| 1 | Satisfaction varies significantly across categories | Score range: 3.66 to 4.55 |
| 2 | Delivery performance is the primary driver | On-time avg: 4.29 stars → 7+ days late avg: 1.70 stars |
| 3 | Seller performance variation is the mechanism | Low-performing sellers have 68% higher late delivery rates |

**The most important takeaway:** 57.3% of delivered orders flow through the weaker half of sellers. So this is not an edge case.

---

## Recommendations


1. **Show seller reliability to buyers**  
   Surface seller quality signals at the point of purchase.

2. **Proactively communicate delivery risk**  
   Flag at-risk orders and update buyers before significant delays happen.

3. **Create a seller performance feedback loop**  
   Share category benchmarks and targeted performance summaries with weaker sellers.

---

## Repository Structure

marketplace-csat-analysis/
├── README.md
├── LICENSE
├── notebook/
│   └── marketplace_csat_analysis.ipynb
├── slides/
│   └── marketplace_slides.pptx
├── data/
│   └── README.md  # Dataset info and download instructions
└── assets/
    └── exec_summary.pdf

---

## Dataset

The Olist dataset is not included in this repository. To reproduce the analysis:

1. Download from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
2. Place the CSV files in a `/data` folder at the project root
3. The notebook expects the path `../data/olist_orders_dataset.csv` etc.

**License:** CC BY-NC-SA 4.0 — cleared for portfolio and non-commercial use.

---

## Limitations

- Dataset covers 2016–2018. Operational conclusions would require current data to validate.
- Seller tier defined by median split as a simplification.
- The analysis is limited to one geography and the repeat purchase signal is weak on this dataset.

---

## About This Project

This case study was completed as part of a Google DA capstone project. It demonstrates end-to-end analytical thinking: from problem framing and data preparation through to stakeholder-ready findings and recommendations.

The analysis was conducted entirely in Python using pandas and Plotly. 
Visualizations are interactive in the Kaggle notebook.