# 🍽 Zomato Dataset — Exploratory Data Analysis (EDA)

This project performs an **Exploratory Data Analysis (EDA)** on the Zomato dataset to uncover insights about restaurant ratings, cuisines, countries, and customer behavior.

---

## 📁 Dataset Information

The dataset contains restaurant information from Zomato across multiple countries.

### Files Used
- `zomato.csv` — Main dataset containing restaurant details  
- `Country-Code.xlsx` — Mapping of country codes to country names  

### Dataset Columns
The dataset includes **21 features**, such as:

- Restaurant ID  
- Restaurant Name  
- Country Code  
- City  
- Address  
- Locality  
- Longitude  
- Latitude  
- Cuisines  
- Average Cost for Two  
- Currency  
- Has Table booking  
- Has Online delivery  
- Is delivering now  
- Switch to order menu  
- Price range  
- Aggregate rating  
- Rating color  
- Rating text  
- Votes  

---

## 🔍 Key Steps in the Analysis

### 1. Data Loading and Inspection
- Loaded the dataset using `latin-1` encoding to avoid UTF-8 decoding errors.
- Inspected data shape, columns, data types, and summary statistics.

### 2. Handling Missing Data
- Found **only 9 missing values** in the `Cuisines` column.
- No other columns had missing values.

### 3. Merging with Country Data
- Merged `zomato.csv` with `Country-Code.xlsx` using `Country Code` as the key.
- Added a new `Country` column for better readability.

### 4. Country-Wise Analysis
- Identified that **India** has the highest number of Zomato records (**8,652**), followed by:
  - United States
  - United Kingdom
- Visualized the top 3 countries using a pie chart.

### 5. Rating Analysis
- Grouped data by:
  - `Aggregate rating`
  - `Rating color`
  - `Rating text`
- Discovered that **over 2,000 restaurants are not rated** (`rating = 0`).
- Created a bar chart to visualize the distribution of ratings.

### 6. Visualization
- Used **Matplotlib** and **Seaborn** for plotting.

#### Plots Include:
- Pie chart for top countries by transaction volume  
- Bar chart for rating distribution  

---

## 📈 Key Observations

### 1. Country Dominance
- India dominates the Zomato dataset with **over 8,600 records**.

### 2. Rating Distribution
- `0.0` (Not rated): 2,148 restaurants  
- `2.5 – 3.4` (Average): Most common rating range  
- `4.5 – 4.9` (Excellent): 61–95 restaurants  

### 3. Cuisine Diversity
- Found **1,825 unique cuisines**.
- The most frequent cuisine is **North Indian**.

---

## 🛠 Technologies Used

- Python  
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
- Jupyter Notebook for interactive analysis

---

## 📄 Conclusion

This EDA provides a foundational understanding of Zomato’s restaurant data by highlighting:

- Key markets  
- Customer rating behavior  
- Cuisine popularity  
- Service availability  

These insights can help inform **business strategy, marketing decisions, and user experience improvements**.


