# Karamoja Food Security Monitoring Tool (2017 Season)

##  Project Overview
Karamoja is the most food-insecure region of Uganda, with persistent droughts, pest outbreaks, and low crop productivity. 
NGOs working in the region lack a clear overview of crop yields and food availability, making it difficult to prioritize interventions.

This project develops a **mock Food Security Monitoring Tool** using:
-  Tableau (interactive dashboard with maps, charts, and filters)
-  Python (Jupyter Notebook for data cleaning and exploratory analysis)

The analysis focuses on the two staple crops of Karamoja:
- Sorghum 
- Maize 

---

##  Dataset Description
The dataset includes **2017 crop season data** provided by Dalberg Data Insights, containing:

- **District-level and Subcounty-level data**
  - Population 
  - Sorghum Yield per Hectare 
  - Maize Yield per Hectare 
  - Crop Area 
  - Sorghum Production 
  - Maize Production 
  - Derived Metric: `Yield_per_Capita` (Kg per person)

- **Geospatial data (Shapefiles)**
  - District Boundaries
  - Subcounty Boundaries
  - Crop Field Maps (Maize and Sorghum)

---

##  Project Workflow
1. **Data Cleaning (Python Notebook)**
   - Renamed columns for clarity
   - Created new derived metrics (e.g., Yield per Capita)
   - Exported cleaned data for Tableau

2. **Exploratory Analysis (Python Notebook)**
   - Visualizations:
     - Boxplots of sorghum vs maize yields
     - Bar chart of yield per capita (district/subcounty)
     - Scatterplots (area vs production efficiency)
     - Stacked bar chart (crop dependency per district)
   - Insights → business recommendations

3. **Visualization & Dashboard (Tableau)**
   - Choropleth map  / Heatmap 
   - Top 10 subcounties by yield per capita
   - Sorghum vs Maize comparison chart
   - KPI cards (Population, Production, Yield per Capita)
   - Interactive filters (Crop Type, District/Subcounty)
   - Here are the **Tableau Public links** for the dashboards :
     - District Dashboard: https://public.tableau.com/app/profile/carl.collins/viz/Project2_17564645247600/District?publish=yes
     - Subcounty Dashboard: https://public.tableau.com/app/profile/carl.collins/viz/Project2_17564645247600/Subcounty?publish=yes
     
4. **Presentation (Slides)**
   - Storytelling with visuals
   - Key findings & recommendations
   - Future work opportunities

---

##  Key Recommendations
1. **Scale Maize as a Reliable Food Source**  
   Maize shows more stability in yields, making it a predictable crop for food security. NGOs should expand maize production as a dependable baseline supply.  

2. **Strengthen Sorghum with Resilient Varieties**  
   Sorghum yields are tightly clustered but vulnerable to drought and pests. Investing in **drought- and pest-resistant sorghum varieties** will safeguard its role as a staple crop.  

3. **Use High-Yield Districts as Redistribution Hubs**  
   Districts such as **Nakapiripirit** and **Kotido**, with high yields per capita, can function as **surplus zones**, redistributing excess production to more food-insecure areas.  

4. **Expand Sorghum Cultivation Area**  
   Since sorghum production correlates strongly with crop area, expanding sorghum acreage in suitable regions can directly increase food supply.  

5. **Balance Crop Strategies for Maximum Production**  
   For districts aiming to maximize output, prioritizing sorghum is effective. However, a balanced approach (≈50/50 sorghum and maize) can reduce risk and ensure steady supply across different conditions.  

---

##  How to Run the Project

### Requirements
- Python 3.x
- Libraries: `pandas`, `matplotlib`, `seaborn`
- Tableau Public

### Steps
1. Clone this repository  
   ```bash
   git clone https://github.com/<your-username>/karamoja-food-security.git
   cd karamoja-food-security
