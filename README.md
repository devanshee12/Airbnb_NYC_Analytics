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
<img width="538" height="374" alt="Screenshot 2025-09-02 at 1 08 41 PM" src="https://github.com/user-attachments/assets/06e8518c-bc48-448a-9bf8-194000f73551" />

 <img width="429" height="347" alt="Screenshot 2025-09-02 at 3 37 10 PM" src="https://github.com/user-attachments/assets/531ed66d-f7ce-4289-a33b-639a0fc6699d" />


### 3. Geospatial Analysis
- Used **GeoPandas** to plot Airbnb listings on a **NYC map**.  
- Visualized distribution of listings and explored high-demand areas.

  
<img width="708" height="532" alt="Screenshot 2025-09-02 at 1 20 38 PM" src="https://github.com/user-attachments/assets/d4b48ee2-7443-4012-9b66-0ec033fbccb6" />

<img width="713" height="495" alt="Screenshot 2025-09-02 at 1 20 13 PM" src="https://github.com/user-attachments/assets/14fcc38f-301e-4b92-96bc-5ccfb3a7c5eb" />



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

<img width="1268" height="782" alt="Screenshot 2025-09-02 at 2 53 53 PM" src="https://github.com/user-attachments/assets/7465b55a-da7b-4418-84e2-c7cd36a0b578" />

<img width="1268" height="782" alt="Screenshot 2025-09-02 at 2 54 42 PM" src="https://github.com/user-attachments/assets/5084d376-bdde-44ea-a96a-77d4b4e2822b" />



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
