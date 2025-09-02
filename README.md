# Airbnb_NYC_Analytics
Analyzed Airbnb listings in New York City to understand pricing trends, availability, and neighborhood demand.
# Airbnb NYC Price & Demand Analysis

## Overview
This project analyzes Airbnb listings in **New York City** to understand **pricing trends, availability, and neighborhood demand**. It demonstrates end-to-end **data analytics skills**, including data cleaning, SQL querying, geospatial analysis, and dashboard visualization using Tableau.

**Tools & Technologies Used:**
- Python (Pandas, GeoPandas, Matplotlib)
- SQL (SQLite / PostgreSQL)
- Tableau Public
- Google Colab

---

## Dataset
- Source: [Inside Airbnb](http://insideairbnb.com/get-the-data.html) – Open Airbnb data  
- Files used: `listings.csv.gz` and `reviews.csv.gz`  
- Focused on **New York City** listings.  
- Cleaned dataset is available in the `data/` folder as `cleaned_listings_ny.csv`.

**Key Columns Used:**
- `neighbourhood_group_cleansed` – Borough  
- `neighbourhood_cleansed` – Neighborhood  
- `latitude`, `longitude` – Listing location  
- `price` – Nightly price  
- `availability_365` – Number of days available  
- `room_type` – Entire home, private room, shared room  

---

## Project Workflow

### 1. Data Cleaning & Preprocessing
- Removed unnecessary columns and null values.  
- Converted `price` to numeric and filtered out extreme outliers.  
- Cleaned neighborhood and borough names for consistency.

### 2. SQL Analysis
- Created a database in SQLite/PostgreSQL.  
- Queries performed:  
  - Average price per neighborhood  
  - Listings count per borough and neighborhood  
  - Average availability per borough  

### 3. Geospatial Analysis
- Used **GeoPandas** to plot Airbnb listings on a **NYC map**.  
- Visualized distribution of listings and explored high-demand areas.  

### 4. Tableau Dashboard
- Built interactive dashboard including:  
  - **Price Heatmap by Neighborhood**  
  - **Availability Map by Neighborhood**  
  - **Listings Count by Borough**  
- Filters included room type, borough, and price range.  
- Insights:  
  - Manhattan has the **highest-priced listings**  
  - Brooklyn has the **most listings**  
  - Certain neighborhoods have **high demand (low availability)**  

---

## Repository Structure
Airbnb_NYC_Analytics/
│
├── notebooks/
│    └── airbnb_analysis.ipynb       # Colab notebook with data cleaning & SQL analysis
│
├── data/
│    └── cleaned_listings_ny.csv    # Cleaned dataset
│
├── tableau/
│    └── airbnb_dashboard.twbx      # Tableau dashboard file
│
└── README.md                       # This file

---

## How to Use
1. Open the notebook in **Google Colab** or **Jupyter Notebook** to run data cleaning and SQL queries.  
2. Open the `cleaned_listings_ny.csv` in **Tableau** to view or edit the dashboard.  
3. Use the filters in Tableau to explore:  
   - Room type  
   - Borough  
   - Price range  

---

## Key Skills Demonstrated
- Data cleaning & preprocessing with **Python & Pandas**  
- SQL queries for analytical insights  
- Geospatial plotting with **GeoPandas**  
- Interactive dashboard creation in **Tableau Public**  
- Data storytelling & visualization  

---

## GitHub Links
- **Notebook:** `notebooks/airbnb_analysis.ipynb`  
- **Dataset:** `data/cleaned_listings_ny.csv`  
- **Tableau Dashboard:** `tableau/airbnb_dashboard.twbx`  

---

## Insights / Summary
- Manhattan has the **highest-priced Airbnb listings**, making it the most premium market.  
- Brooklyn has the **largest number of listings**, indicating high supply.  
- Neighborhoods with **low availability** signal **high demand**, useful for hosts and analysts.  

---

## License
This project is **open-source** and for learning purposes.
