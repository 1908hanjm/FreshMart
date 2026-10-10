# 🥩 FreshMart — Meat Demand & Waste Reduction

A business case study analyzing day-of-week demand patterns and spoilage risk in a grocery meat department — turning perishable inventory data into ordering decisions that cut waste.

## 📌 Project Overview

- **Business Problem**: FreshMart's meat department over-orders on slow days and stocks out on peak days. Spoilage eats into margins.
- **Goal**: Analyze demand patterns by weekday, category, and store — then recommend order quantities that minimize waste without losing sales.
- **Dataset**: [Kaggle — Perishable Goods Management](https://www.kaggle.com/datasets/likithagedipudi/perishable-goods-management) (100,000 synthetic transaction records, 2023–2024, 50 stores × 5 US regions, 10 product categories)
- **Tools**: Python (pandas, NumPy, matplotlib, seaborn), Jupyter Notebook, Tableau
- **Interactive Dashboard**: [FreshMart Meat Demand & Waste Reduction (Tableau Public)](https://public.tableau.com/app/profile/dave.han6326/viz/FreshMartMeatDemandWasteReduction/MeatWeekdayDemandvsWaste)

## 🔍 Key Findings

| Metric | Value |
|---|---|
| Meat avg waste rate | **18.2%** |
| Weekday waste vs weekend | **~20%** vs **~13%** |
| Meat waste cost | **$3.5M** (45% of meat profit) |
| Markdown margin | **−17%** (applied too late, median 2 days to expiry) |
| Simulated saving (right-sized weekday orders) | **~$1.09M** (30.9% of meat waste cost) |

**Insights:**
1. **Weekday over-ordering drives waste** — orders stay flat (~255 units) while demand drops on weekdays (~207 sold) vs weekends (~229 sold).
2. **Markdowns backfire** — applied at a median of 2 days to expiry, they lose 17% margin instead of preventing waste.
3. **Simulation** — matching weekday order buffers to weekend levels cuts weekday waste from ~20% to ~12.5%.

## 📁 Repository Structure

```text
FreshMart/
├── notebooks/
│   ├── 01_data_cleaning.ipynb   # Data audit, missing values, date handling
│   ├── 02_eda.ipynb             # Day-of-week demand patterns, category & regional analysis
│   └── 03_waste_analysis.ipynb  # Order-quantity simulation & recommendations
├── .gitignore
└── README.md
```

## 🚀 How to Run

1. Download the dataset from the Kaggle link above.
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Open the notebooks in order, or click "Open in Colab".
