# 🥩 FreshMart — Meat Demand & Waste Reduction

A business case study analyzing day-of-week demand patterns and spoilage risk in a grocery meat department — turning perishable inventory data into ordering decisions that cut waste.

## 📌 Project Overview

- **Business Problem**: FreshMart's meat department over-orders on slow days and stocks out on peak days. Spoilage eats into margins.
- **Goal**: Analyze demand patterns by weekday, category, and store — then recommend order quantities that minimize waste without losing sales.
- **Dataset**: [Kaggle — Perishable Goods Management](https://www.kaggle.com/datasets/likithagedipudi/perishable-goods-management) (100,000 synthetic transaction records, 2023–2024, 50 stores × 5 US regions, 10 product categories)
- **Tools**: Python (pandas, NumPy, matplotlib, seaborn), Jupyter Notebook, Tableau

## 📁 Repository Structure

```text
FreshMart/
├── notebooks/
│   ├── 01_data_cleaning.ipynb   # Data audit, missing values, date handling
│   ├── 02_eda.ipynb             # Day-of-week demand patterns, category & regional analysis
│   └── 03_waste_analysis.ipynb  # Spoilage risk scoring & order-quantity recommendations
├── .gitignore
└── README.md
```

## 🚀 How to Run

1. Download the dataset from the Kaggle link above.
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Open the notebooks in order, or click "Open in Colab".
