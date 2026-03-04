# AgriculturalPrice-YieldAnalysis

This project analyzes USDA produce pricing and yield data across 2020 and 2022, merged with US GDP data, to uncover patterns in how produce form, price tier, and category relate to one another during a period of significant economic change.


## 📁 Dataset Overview
Four USDA datasets covering fruit and vegetable retail prices and yields across two years, combined with World Bank US GDP data. The merged dataset contains:

- 310 records across 119 unique produce items
- Features including retail price, cup equivalent price, yield, produce form, and category
- Years 2020 and 2022, spanning a 21.5% US GDP growth period


## 🎯 Objective
The main objectives of this analysis are:
- Identify the most frequently purchased produce items
- Analyze common produce item combinations (e.g., apples and bananas often bought together)
- Visualize trends and patterns that can inform retail decisions


## 📈 Analysis Workflow
1. **Import Libraries**  
   Standard data science libraries like `pandas`, `matplotlib`, and `seaborn` were used.

2. **Data Cleaning and Preparation**  
   - Combined rows or columns to create transaction baskets  
   - Handled missing values and duplicates

3. **Exploratory Data Analysis (EDA)**  
   - Most common produce items
   - Co-occurrence heatmaps of item pairs
   - Visualizations for frequency distributions

4. **Pattern Discovery**  
   - Used association rule mining (e.g., Apriori algorithm from `mlxtend`)
   - Calculated support, confidence, and lift for popular item pairs


## 📊 Key Results
- **Top Purchased Items**: Apples, Bananas, Tomatoes, and Carrots
- **Common Combos**: Bananas & Strawberries, Lettuce & Tomatoes
- **Insights**:
  - High lift values between certain item pairs suggest strong co-purchasing behavior
  - Potential for bundling or co-promotions in stores


## 📌 Conclusions
- Several produce items consistently appear together in transactions, indicating stable consumer behavior.
- Association rules can help guide marketing strategies like combo deals or aisle layouts.
