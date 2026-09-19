# 🏠 Airbnb Listings — Data Cleaning, EDA & Interactive Dashboard

![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)
![Chart.js](https://img.shields.io/badge/Chart.js-Interactive%20Dashboard-FF6384?logo=chart.js&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-Environment-F9AB00?logo=googlecolab&logoColor=white)

An end-to-end data analysis project on a real-world, messy Airbnb listings dataset — cleaned
and explored in Python, then visualized in a standalone interactive HTML dashboard.

## 📑 Table of Contents
- [Tech Stack & Tools](#️-tech-stack--tools)
- [Dataset](#-dataset)
- [Core Workflow](#-core-workflow)
- [Key Insights](#-key-insights)
- [Interactive Dashboard](#-interactive-dashboard)
- [Repository Structure](#-repository-structure)
- [How to Run](#-how-to-run-the-notebook)

## 🛠️ Tech Stack & Tools
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, ydata-profiling
- **Dashboard:** HTML/CSS/JS (Chart.js)

## 📊 Dataset
14,456 scraped Airbnb listings, 13 raw columns — name, rating, reviews, host info, address,
features, amenities, safety/house rules, images, and price.

## 🔍 Core Workflow

<details>
<summary><strong>1. Data Cleaning</strong> — 14,456 → 10,913 rows (click to expand)</summary>
<br>

Handled missing values, duplicate listings, and unrecoverable host records — a ~24.5%
reduction from the raw dataset to a fully analysis-ready one.
</details>

<details>
<summary><strong>2. Feature Engineering</strong></summary>
<br>

Parsed country from address, extracted check-in/check-out times from house rules, converted
price and review counts to numeric types, and standardized amenity lists (filtering out
"Unavailable" entries so only actually-offered amenities are counted).
</details>

<details>
<summary><strong>3. Exploratory Data Analysis</strong> — 10 business questions</summary>
<br>

Covered country distribution, rating patterns, amenities, price vs. guest capacity,
check-in/out norms, and house-rule trends across countries.
</details>

<details>
<summary><strong>4. Interactive Dashboard</strong></summary>
<br>

Built a standalone HTML dashboard (<code>airbnb_dashboard.html</code>) summarizing the key
findings, with an interactive line/bar toggle on the pricing chart.
</details>

## 📈 Key Insights

| Metric | Finding |
|---|---|
| 🌍 Top country | India — **~19%** of all cleaned listings |
| ⭐ Unrated listings | **~17.4%** still marked `New` |
| 💰 Price ↔ guests | **0.35** correlation; ~11x price range (1 → 16 guests) |
| 🛋️ Top amenities | Wifi, Kitchen, Free parking — offered on **70%+** of listings |
| 📜 House rules | **Japan** strictest across all 3 rule types; **India** most permissive |

## 📺 Interactive Dashboard

The notebook's final cell renders a full interactive dashboard inline — KPI cards, a
line/bar-toggle pricing chart, top countries, top amenities, and a house-rules-by-country
table. It's also included as a standalone file (`airbnb_dashboard.html`) you can open
directly in any browser, or host via GitHub Pages for a shareable link.

## 📁 Repository Structure

```text
DA-AIRBNB-PROJECT/
├── README.md
├── DA_AIRBNB.ipynb
├── airbnb_dashboard.html
└── data/
    └── airbnb.csv
```

## 🚀 How to Run the Notebook
1. Clone this repository (the notebook pulls `data/airbnb.csv` from it automatically):
   ```bash
   git clone https://github.com/mdooo7/DA-AIRBNB-PROJECT
   ```
2. Open `DA_AIRBNB.ipynb` in Google Colab (or upload it to Colab directly).
3. Run all cells sequentially: **Runtime → Run all** — the last cell renders the interactive
   dashboard inline.

Alternatively, open `airbnb_dashboard.html` directly in a browser, or host it via GitHub Pages
for a shareable link.
