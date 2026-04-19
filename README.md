# 💊 Pharma Retail & Customer Insight Dashboard

---

## 📌 Title

**Pharma Retail & Customer Insight Dashboard**  
*An end-to-end Market Intelligence project — from raw transactional data to strategic business recommendations*

**Tools**: Microsoft Excel · Power Query · Power BI Desktop  
**Dataset**: 116,737 pharmacy retail transactions | Sep–Nov 2021  
**Deliverable**: 4-page interactive Power BI report

---

## 🧭 Executive Summary

This project delivers a comprehensive market intelligence analysis of a pharmaceutical retail network,
covering 9 stores across 2 distribution chains over a 3-month period.

Starting from a raw, uncleaned transactional dataset, the analysis follows a full end-to-end
analytics workflow: data quality assessment, systematic cleaning, feature engineering, and
interactive visualization — culminating in concrete business recommendations.

The dashboard is structured across three strategic lenses:
- **Who** is buying → Customer Segmentation
- **What** is selling → Product Volume Analysis
- **Where** performance gaps exist → Distribution Performance

Key finding: a single customer segment (women aged 31–40) and a single product category
(NonMedication, 97.71% of revenue) drive the vast majority of network performance —
creating a clear strategic opportunity for targeted intervention.

---

## ❓ Business Problem

Pharmaceutical retail networks generate large volumes of transactional data daily,
but this data is rarely translated into actionable intelligence at the store or chain level.

This project addresses three core business questions:

**1. Customer Intelligence**
> *Who is our core customer, and are we allocating marketing resources toward the highest-value segments?*

**2. Product Strategy**
> *Which product categories drive revenue, and are our inventory and promotional strategies aligned with actual demand?*

**3. Distribution Efficiency**
> *Which stores and chains are underperforming relative to the network average, and what operational levers can close the gap?*

Without answers to these questions, marketing budgets are misallocated, stockouts occur in
high-demand locations, and underperforming stores go unaddressed — all leading to measurable
revenue loss.

---

## 📐 Methodology

### Phase 1 — Data Cleaning & Preparation (Excel + Power Query)

The raw dataset presented multiple data quality issues, each systematically resolved:

| Issue | Solution |
|---|---|
| Date stored as text (DD.MM.YYYY) | Converted using `it-IT` locale settings in Power Query |
| Numeric values with space as thousands separator (`2 784,38`) | Removed spaces via Find & Replace before type conversion |
| Age outliers (range: 3–97) | Filtered to 18–90 to ensure demographic integrity |
| No customer segmentation by age | Engineered `age_bin` feature: 18–30, 31–40, 41–50, 51–60, 61–70, 71+ |

### Phase 2 — Interactive Dashboard (Power BI Desktop)

Built a 4-page Power BI report with cross-page interactivity via Chain slicer:

| Page | Content | Visual Types |
|---|---|---|
| Overview | KPI summary — Revenue, Transactions, Unique Customers | 3 KPI Cards |
| Customer Segmentation | Gender and age group revenue distribution | Donut Chart, Clustered Column Chart |
| Product Volume Analysis | Category mix by store and overall | Stacked Column Chart, Donut Chart |
| Distribution Performance | Store ranking and chain trend comparison | Treemap, Line Chart, Slicer |

---

## 🛠️ Skills Demonstrated

**Data Analytics**
- ✅ End-to-end data pipeline: raw dataset → cleaned data → interactive dashboard
- ✅ Data quality assessment and systematic cleaning in Power Query
- ✅ Feature engineering (Age Bins) for improved analytical readability
- ✅ Multi-dimensional segmentation analysis (demographic + product + geographic)

**Business Intelligence**
- ✅ KPI definition and dashboard design for non-technical stakeholders
- ✅ Retail network performance benchmarking across stores and chains
- ✅ Revenue trend analysis and anomaly identification
- ✅ Business-oriented data storytelling and insight communication

**Marketing & Strategy**
- ✅ Customer profiling and value-based segmentation
- ✅ Product mix analysis and demand pattern identification
- ✅ Translation of data findings into actionable marketing recommendations
- ✅ Strategic prioritization of resources based on revenue concentration

---

## 📈 Results & Business Recommendations

### Finding 1 — Customer Segmentation

**Data says:**
Women represent **76% of total revenue** (€85.56M vs €27.01M for men).
The 31–40 female cohort is the single highest-revenue segment across all stores and chains.
The 18–30 segment shows strong volume but lower average ticket — indicating price sensitivity.

**Business Recommendation:**
> Implement a **two-tier loyalty programme**: a premium tier targeting the 31–40 female segment
> with personalized offers on high-margin NonMedication products (beauty, wellness, supplements),
> and an acquisition tier for the 18–30 cohort offering entry-level incentives to increase
> purchase frequency and basket size over time.
>
> This approach mirrors strategies successfully deployed in health & beauty retail
> and could be piloted in the top 3 stores before network-wide rollout.

---

### Finding 2 — Product Volume Analysis

**Data says:**
NonMedication products account for **97.71% of total revenue** (€109.98M).
Medication represents only **2.29%** (€2.58M) — despite typically carrying higher unit margins.

**Business Recommendation:**
> The near-total dominance of NonMedication revenue signals that this network has significant
> untapped potential in the **prescription and OTC medication segment**.
>
> A targeted **pharmacy activation strategy** could include: in-store pharmacist consultation
> services, seasonal health campaigns (flu prevention, vitamin supplementation), and partnerships
> with local GPs to drive prescription foot traffic.
>
> Even a modest shift of 5% of current NonMedication customers toward Medication purchases
> could generate an estimated **€5.5M+ in incremental revenue** — at likely higher margins
> than the current parapharmacy model.

---

### Finding 3 — Distribution Performance

**Data says:**
Name6, Name7 and Name5 generate **over 60% of total network revenue**.
Name0 and Name8 are the lowest performers, each generating less than €4M over 3 months.
Chain B shows **accelerating growth** vs Chain A between October and November 2021,
including notable revenue spikes in late November suggesting a promotional or seasonal effect.

**Business Recommendation:**
> Apply a **portfolio approach** to store management:
>
> - **Invest** in Name6, Name7 and Name5 — increase inventory depth, expand store footprint
>   or opening hours, and run exclusive loyalty events to consolidate their market leadership.
>
> - **Diagnose** Name0 and Name8 — conduct a root cause analysis comparing local demographics,
>   competition density, and store assortment vs top performers. Underperformance at this scale
>   may indicate a location mismatch or assortment gap that can be corrected.
>
> - **Replicate Chain B's growth drivers** — identify the operational or promotional mechanics
>   behind Chain B's November acceleration and systematically apply them across Chain A locations
>   to close the performance gap before the next seasonal peak.

---

## 📁 Repository Structure

```
pharma-retail-dashboard/
│
├── data/
│   └── pharmaceutical_sales_clean.xlsx    # Cleaned dataset with Power Query steps
│
├── powerbi/
│   └── pharma_dashboard.pbix              # Power BI dashboard file
│
├── screenshots/
│   ├── 01_overview.png
│   ├── 02_customer_segmentation.png
│   ├── 03_product_volume_analysis.png
│   └── 04_distribution_performance.png
│
├── export/
│   └── pharma_dashboard.pdf               # Full report export
│
└── README.md
```

## 🚀 How to Open the Dashboard

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone or download this repository
3. Open `pharma_dashboard.pbix` in Power BI Desktop
4. All data is embedded — no external connection required

---

*Developed by Bilel Ben Boulaares | Università degli studi di Modena e Reggio Emilia | 2026
*📧 [bbenboulaaresbilel@gmail.com] | 🔗 https://www.linkedin.com/in/bilel-ben-boulaares-15702b374/
