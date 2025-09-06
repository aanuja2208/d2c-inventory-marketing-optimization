# Data-Driven Optimization of Inventory and Marketing for a D2C Artisanal Brand

This project implements a comprehensive Business Data Management (BDM) pipeline for analysing sales, returns, and customer journey data from Hastvikas, a Direct-to-Consumer (D2C) artisanal brand. It applies descriptive analytics, machine learning, and forecasting to optimise catalog visibility, predict return risks, segment products, and plan inventory demand.

---

## Project Overview

The project develops a modular analytics framework that combines descriptive and predictive methods to address key operational challenges faced by a small but growing e-commerce brand.

- **Data Sources:** Data cleaning → Funnel & returns analysis → NLP-based query matching → SKU clustering → Time series forecasting
- **Pipeline**: Data cleaning → Sentiment analysis → Keyword extraction → Visualization  
- **Outcome**: Built an integrated decision-support system enabling proactive inventory planning and marketing optimisation 
- **Execution**: Fully script-driven, reproducible analysis with structured visual reporting

---

## Tech Stack

- **Language**: Python 3, Excel  
- **Libraries**: Pandas, Scikit-learn, Statsmodels, Matplotlib, NLTK  
- **ML Models**: Logistic Regression (return risk), K-Means Clustering (SKU segmentation), SARIMA (time series forecasting)  
- **NLP**: TF-IDF & Cosine Similarity (query–catalog matching)  
- **Visualisation**: Funnel charts, Pareto charts, heatmaps, PCA scatterplots, and time series plots  
- **Data Format**: CSV (orders, returns, product catalog, customer queries) 

---

## Key Features

- **Catalog Discoverability**  
  TF-IDF & cosine similarity to match customer search queries with catalog metadata.  

- **Customer Funnel Analysis**  
  Drop-off analysis across sessions → cart → checkout → purchase, with revenue leakage simulation.  

- **Return Risk Prediction**  
  Logistic regression to flag SKUs with return ratios >15%, integrated into restocking decisions.  

- **Product Segmentation**  
  K-Means clustering with PCA visualisation to group SKUs into promote / investigate / caution categories.  

- **Demand Forecasting**  
  SARIMA model to forecast weekly orders (8 weeks ahead). 

---
## Project Structure
```text
d2c-inventory-marketing-optimizer/
├── data/ # Raw & processed datasets (orders, returns, queries, catalog)
├── scripts/
│ ├── query_matching.py # TF-IDF + cosine similarity for catalog optimisation
│ ├── funnel_analysis.py # Customer journey drop-off & simulation
│ ├── return_risk.py # Logistic regression for return prediction
│ ├── product_segmentation.py # K-Means clustering + PCA visualisation
│ └── demand_forecast.py # SARIMA-based weekly order forecasting
├── visuals/ # Generated plots & dashboards
│ ├── funnel_chart.png
│ ├── return_risk_matrix.png
│ ├── sku_clusters.png
│ ├── weekly_forecast.png
│ └── query_alignment_heatmap.png
├── reports/ # Mid-term and final reports (PDF)
│ ├── mid_term_report.pdf
│ └── final_submission.pdf
├── requirements.txt # Python dependencies
└── README.md # Project overview and instructions
```

---

## Screenshots


### 1. Search Query–Catalog Alignment  
Visualisation of query-to-product similarity matrix with action flags.  
![Search Query Heatmap](visuals/query_alignment_heatmap.png)  

---

### 2. Customer Funnel Drop-Offs  
Stage-wise breakdown showing steep conversion leakage.  
![Funnel Chart](visuals/funnel_chart.png)  

---

### 3. Return Risk Classification  
Confusion matrix output for logistic regression return prediction.  
![Return Risk Matrix](visuals/return_risk_matrix.png)  

---

### 4. Product Segmentation Clusters  
PCA scatter plot of SKUs grouped into 3 behavioural clusters.  
![SKU Clusters](visuals/sku_clusters.png)  

---

### 5. Weekly Demand Forecasting  
SARIMA forecast showing order growth trend over 8 weeks.  
![Weekly Forecast](visuals/weekly_forecast.png)  


<p align="center">
  <img src="Screenshots/dashboard_summary.png.png" width="800" alt="Dashboard Summary Visualization">
</p>
