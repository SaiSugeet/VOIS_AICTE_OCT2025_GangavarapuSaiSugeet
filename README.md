# 🏨 Airbnb Data Analytics & Visualization Project

This project analyzes Airbnb booking/listing data using **Python, Pandas, Seaborn, Plotly, and Scikit-learn**.  
The goal is to uncover insights into **booking patterns, pricing strategies, guest preferences, and host performance**, while also building a **simple predictive model** for service fees.

---

## 📌 Objectives
1. **Booking Patterns** → Identify seasonal trends, location variations, and listing availability.  
2. **Pricing Strategies** → Analyze price distributions, neighborhood-wise price differences, and impact of reviews on price.  
3. **Guest Preferences** → Explore room type distribution, popular neighborhoods, and house rules (via word cloud).  
4. **Host Performance** → Evaluate top hosts, responsiveness, and identity verification status.  
5. **Predictive Modeling** → Build a baseline regression model to predict `service_fee`.  
6. **Additional Visuals for PPT & Demo**:  
   - 📊 **Correlation Heatmap** (relationships between numeric features).  
   - 🗺️ **Interactive Map** (listings plotted geographically, colored by price/service fee).  

---

## 🛠️ Tech Stack
- **Language**: Python 3  
- **Libraries**:  
  - Data Handling → `pandas`, `numpy`  
  - Visualization → `seaborn`, `matplotlib`, `plotly`, `wordcloud`  
  - Machine Learning → `scikit-learn` (Linear Regression)  
  - Mapping → `plotly.express` (`scatter_mapbox`)  
- **Environment**: Google Colab (recommended) / VS Code (optional)  

---

## 📂 Dataset
- File: `Airbnb_Data.xlsx`  
- Sheet: `"in"`  
- Columns include: `id`, `name`, `host_id`, `host_name`, `neighbourhood group`, `neighbourhood`, `lat`, `long`, `room type`, `price`, `service fee`, `availability 365`, etc.  

🔧 **Preprocessing steps:**  
- Removed duplicates & null values.  
- Cleaned numeric columns (`price`, `service_fee`).  
- Fixed spelling errors (e.g., "brookln" → "Brooklyn").  
- Converted dates (`last_review`).  
- Standardized column names (`availability 365` → `availability_365`, etc.).  
- Removed outliers (availability > 365).  

---

## 📊 Analysis & Visualizations
### 1. Booking Patterns
- Distribution of listing availability.  
- Review activity trends over time.  
- Listings share by neighborhood group.  

### 2. Pricing Strategies
- Price distribution & outliers.  
- Average price by neighborhood group.  
- Scatter plot of price vs number of reviews.  

### 3. Guest Preferences
- Room type distribution.  
- Top neighborhoods by listing count.  
- Word cloud of house rules.  

### 4. Host Performance
- Top hosts by listing count.  
- Host identity verification status.  
- Relationship between host listings and availability.  

### 5. Extra Visuals
- 🔗 **Correlation Heatmap** (numeric relationships such as price vs reviews vs availability).  
- 🗺️ **Interactive Map** (listings plotted on city map with hover info).  

### 6. Predictive Modeling
- Linear Regression model to predict `service_fee`.  
- Evaluation metrics: **Mean Squared Error (MSE)**, **R² Score**.  
- Plot: Actual vs Predicted Service Fee.  

---
