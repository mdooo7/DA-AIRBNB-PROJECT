# Airbnb Listings — Data Cleaning, EDA & Interactive Dashboard

An end-to-end data analysis project on a real-world, messy Airbnb listings dataset — cleaned
and explored in Python, then visualized in an interactive HTML dashboard.

## 🛠️ Tech Stack & Tools
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, ydata-profiling
- **Dashboard:** HTML/CSS/JS (Chart.js)

## 📊 Dataset
14,456 scraped Airbnb listings, 13 raw columns — name, rating, reviews, host info, address,
features, amenities, safety/house rules, images, and price.

## 🔍 Core Workflow
1. **Data Cleaning:** Handled missing values, duplicate listings, and unrecoverable host
   records, reducing the raw dataset from 14,456 to 10,913 clean rows (~24.5% removed).
2. **Feature Engineering:** Parsed country from address, extracted check-in/check-out times
   from house rules, converted price and review counts to numeric types, and standardized
   amenity lists.
3. **Exploratory Data Analysis:** Answered 10 business questions covering country
   distribution, rating patterns, amenities, price vs. guest capacity, check-in/out norms,
   and house-rule trends across countries.
4. **Interactive Dashboard:** Built a standalone HTML dashboard (`airbnb_dashboard.html`)
   summarizing the key findings, with an interactive line/bar toggle on the pricing chart.

## 📈 Key Insights
- India accounts for ~19% of all cleaned listings — the single largest country, followed by Italy and Greece.
- ~17.4% of listings are still unrated (`New`); the remaining ~83% skew toward high ratings.
- Guest capacity has a moderate positive correlation (0.35) with price, and roughly an 11x price range between 1-guest and 16-guest listings.
- Wifi, Kitchen, and Free parking are offered on over 70% of listings — the clear baseline guest expectation.
- House-rule enforcement (smoking, parties, pets) varies sharply by country — Japan is strictest across all three rule types, India the most permissive among high-volume countries.

## 🚀 How to Run the Notebook
1. Clone this repository (the notebook pulls `data/airbnb.csv` from it automatically):
   ```
   git clone https://github.com/mdooo7/DA-AIRBNB-PROJECT
   ```
2. Open `DA_AIRBNB.ipynb` in Google Colab (or upload it to Colab directly).
3. Run all cells sequentially: **Runtime → Run all** — the last cell renders the interactive dashboard inline.

Alternatively, open `airbnb_dashboard.html` directly in a browser, or host it via GitHub Pages
for a shareable link.
