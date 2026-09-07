# Airbnb Listings — Data Cleaning & Exploratory Data Analysis

An end-to-end data analysis project on a real-world, messy Airbnb listings dataset — built in
Google Colab to clean structural data flaws and answer 10 business questions about pricing,
ratings, amenities, and booking-rule patterns across countries.

## 🛠️ Tech Stack & Tools
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, ydata-profiling

## 🔍 Core Workflow
1. **Data Cleaning:** Handled missing values, duplicate listings, and unrecoverable host
   records, reducing the raw dataset from 14,456 to 10,913 clean rows (~24.5% removed).
2. **Feature Engineering:** Parsed country from address, extracted check-in/check-out times
   from house rules, converted price and review counts to numeric types, and standardized
   amenity lists.
3. **Exploratory Data Analysis:** Answered 10 targeted questions covering country distribution,
   rating patterns, amenities, price vs. guest capacity, check-in/out norms, and house-rule
   trends — including two visualizations (rule patterns by country, price trends by guest count).

## 📈 Key Insights
- India accounts for ~29% of all listings — the single largest market in the dataset.
- Ratings are polarized: perfect 5.0s and un-rated "New" listings together make up ~40% of
  listings, rather than a smooth distribution.
- Guest capacity and price show a moderate positive correlation (0.31), with a ~25x price
  range between 1-guest and 16-guest listings.
- ~44% of listings are still unrated, a meaningful trust gap for new hosts.

## 🚀 How to Run the Notebook
1. Clone this repository (the notebook pulls `data/airbnb.csv` from it automatically):
   git clone https://github.com/mdooo7/DA-AIRBNB-PROJECT
3. Open `DA_AIRBNB.ipynb` in Google Colab (or upload it to Colab directly).
4. Run all cells sequentially: **Runtime → Run all**.
