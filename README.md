# 🚗 Regional Vehicle Sales Analysis — India
### FY2019–FY2024 | Data Analytics Project

A comprehensive analysis of **131.8 million vehicle sales** across 28 Indian states, 5 segments, and 6 financial years — uncovering demand patterns, high-growth markets, and the EV revolution.

---

## 🌐 Live Dashboard

Open `dashboard.html` in any browser — no server needed, no installation, works offline.

**Or view on GitHub Pages:** `https://<your-username>.github.io/<repo-name>/dashboard.html`

---

## 📁 Project Structure

```
├── dashboard.html                    ← Main frontend (open this!)
├── README.md                         ← This file
├── india_vehicle_sales.ipynb         ← Complete Jupyter notebook (63 cells)
├── DATA_DICTIONARY.md                ← Column reference + sources
│
├── data/
│   ├── india_vehicle_sales_raw.csv   ← Raw dataset (with quality issues)
│   ├── india_vehicle_sales_cleaned.csv ← Clean dataset (3,360 rows × 10 cols)
│   ├── india_vehicle_sales_kpis.csv  ← Engineered KPIs (YoY, CAGR, market share)
│   └── state_market_tiers.csv        ← KMeans cluster output (28 states × 4 tiers)
│
└── charts/                           ← All 15 analysis charts (PNG)
    ├── t21a_units_sold_distribution.png
    ├── t21b_total_sales_by_segment.png
    ├── t22a_top10_states_total_sales.png
    ├── t22b_segment_mix_by_region.png
    ├── t22c_state_segment_heatmap.png
    ├── t23a_national_yoy_trend.png
    ├── t23b_segment_yoy_trend.png
    ├── t27_top15_states_horizontal.png
    ├── t28_segment_breakdown_top10.png
    ├── t29_state_year_heatmap.png
    ├── bq5_ev_adoption_by_state.png
    ├── bq6_fuel_type_shift.png
    ├── bq7_oem_market_share.png
    ├── t32_kmeans_state_clusters.png
    └── t33_sales_forecast.png
```

---

## 📊 What's Inside

### Dataset
- **3,360 rows** × 10 columns after cleaning
- **5 segments:** Two-Wheeler, Three-Wheeler, Passenger Car, Commercial Vehicle, Electric Vehicle
- **28 states** across 6 regions (North, South, East, West, Central, Northeast)
- **6 financial years:** FY2019–FY2024
- **18 OEMs** including Hero MotoCorp, Maruti Suzuki, Tata Motors, Bajaj Auto
- Anchored to **SIAM Annual Reports** + **VAHAN Dashboard** real national totals (within ±3.5%)

### 8 Business Questions Answered
| Category | Questions |
|---|---|
| Regional Demand | BQ1: Which states/regions lead? BQ2: Fastest growing markets? |
| Segment & Mix | BQ3: How does mix differ by region? BQ4: Which segments grow/decline? |
| EV & Fuel | BQ5: EV adoption by state? BQ6: Fuel type shift over time? |
| OEM & Market | BQ7: OEM market share by segment? BQ8: Strategic recommendations? |

### Key Findings
- 🔴 **EV grew +2,430%** — 64K units (FY2019) → 1.62M (FY2024)
- 🔵 **North region = 31.2%** of national sales (driven by UP's 2W market)
- 🟢 **Maruti Suzuki = 49% PV** | Hero MotoCorp = 34% 2W | Tata Motors = 49% EV
- 🟡 **Two-Wheelers declining -13.6%** — only segment below FY2019 levels
- ⚡ **Maharashtra EV CAGR = 103.8%** over 3 years
- 📈 **Forecast:** FY2025 = 32.8M units | FY2026 = 41.9M units (R²=0.978)

### Advanced Analysis
- **KMeans Clustering (k=4):** 28 states grouped into Metro Giants, Large Markets, Mid Markets, Emerging
- **Polynomial Regression (degree=2):** Sales forecast with R²=0.978, capturing COVID dip + recovery

---

## 🛠️ Tech Stack

```
Python 3.11    Pandas 3.0    NumPy 2.4    Matplotlib 3.10
Seaborn 0.13   Scikit-learn 1.8          Jupyter Notebook
HTML5 / CSS3 / Vanilla JS    Chart.js 4.4
```

---

## 🚀 How to Run

### Option 1 — Just open the dashboard
```bash
# No installation needed
open dashboard.html    # Mac
start dashboard.html   # Windows
```

### Option 2 — Run the Jupyter notebook
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook india_vehicle_sales.ipynb
```

### Option 3 — GitHub Pages
1. Push this repo to GitHub
2. Go to Settings → Pages → Deploy from branch (main, root)
3. Visit `https://<username>.github.io/<repo>/dashboard.html`

---

## 📚 Data Sources

| Source | What it provided |
|---|---|
| [SIAM Annual Reports](https://www.siam.in) | National segment totals FY2019–FY2024 |
| [VAHAN Dashboard](https://vahan.parivahan.gov.in) | State-wise EV registration patterns |
| OEM Annual Reports | Manufacturer market share figures |

---

## 📄 Deliverables

| File | Description |
|---|---|
| `dashboard.html` | Interactive frontend — single file, works offline |
| `india_vehicle_sales.ipynb` | Complete notebook — Steps 1–12, 63 cells |
| `RVSA_Project_Report.docx` | 7-section professional report with embedded charts |
| `RVSA_Presentation.pptx` | 12-slide deck with professional design |
| `india_vehicle_sales_cleaned.csv` | Final clean dataset |
| `india_vehicle_sales_kpis.csv` | Engineered KPI columns |
| `DATA_DICTIONARY.md` | Full column documentation |

---

*Data Analytics Course Project · Regional Vehicle Sales Analysis · India*
