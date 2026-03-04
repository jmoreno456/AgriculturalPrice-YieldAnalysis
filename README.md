# AgriculturalPrice-YieldAnalysis

This project analyzes USDA produce pricing and yield data across 2020 and 2022, merged with US GDP data, to uncover patterns in how produce form, price tier, and category relate to one another during a period of significant economic change.


## 📁 Dataset Overview
Four USDA datasets covering fruit and vegetable retail prices and yields across two years, combined with World Bank US GDP data. The merged dataset contains:

- 310 records across 119 unique produce items
- Features including retail price, cup equivalent price, yield, produce form, and category
- Years 2020 and 2022, spanning a 21.5% US GDP growth period


## 🎯 Objective
The main objectives of this analysis are:
- Identify statistically significant relationships between pricing, yield, and produce characteristics
- Compare pricing and yield patterns between fruits and vegetables across two years
- Discover association rules linking produce form and price tier to category membership


## 📈 Analysis Workflow
1. **Data Merging and Preparation**  
   Merged four USDA CSVs and US GDP data into a unified pipeline using pandas

2. **Exploratory Data Analysis (EDA)**  
   Generated regression plots comparing retail price vs yield (vegetables) and cup equivalent size vs yield (fruits) for both years using seaborn

3. **Correlation Analysis**  
   Computed R² and p-values using scipy to assess statistical significance of observed relationships

4. **Association Rule Mining**  
   Binned prices into tiers and encoded produce attributes as transactions, then ran Apriori (mlxtend) to extract rules filtered by support, confidence, and lift


## 📊 Key Results
- **Top Purchased Items**: Apples, Bananas, Tomatoes, and Carrots
- **Common Combos**: Bananas & Strawberries, Lettuce & Tomatoes
- **Insights**:
  - High lift values between certain item pairs suggest strong co-purchasing behavior
  - Potential for bundling or co-promotions in stores


## 📌 Conclusions
- Several produce items consistently appear together in transactions, indicating stable consumer behavior.
- Association rules can help guide marketing strategies like combo deals or aisle layouts.
