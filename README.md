# World Happiness Report - Exploratory Data Analysis (EDA)

This project explores the **World Happiness Report** data (2011–2024) to uncover insights about factors that influence happiness across countries. The dataset includes indicators like GDP per capita, social support, healthy life expectancy, freedom, generosity, corruption perception, and more.

> **Goal:** Explore factors influencing global happiness using data from 2011–2024, and provide insights for decision-makers.

## Exploratory Data Analysis Strategy

We'll investigate:
- How different variables correlate with the Happiness Score
- Which features are the strongest predictors of happiness
- How top-performing countries differ from those with lower scores

We aim to identify the *most influential factors* and assess which ones can be targeted by governments or organizations to improve well-being.


## Dataset Overview
Source: World Happiness Report
Years Covered: 2011 to 2024
---

## 🗂️ Project Overview

This project analyzes the **World Happiness Report** to uncover trends and relationships across countries. The dataset includes key indicators:

- GDP per capita
- Social support
- Healthy life expectancy
- Freedom to make life choices
- Generosity
- Perceptions of corruption
---

## Key Insights

> **Countries with higher GDP per capita and social support tend to have higher happiness scores.**  
> **Corruption perception and freedom contribute significantly to regional differences.**  
> **Healthy life expectancy is a consistent and strong predictor of happiness.**  
> **Top happiest countries are consistently located in Northern and Western Europe.**  
> **Least happy countries are often in conflict zones or face economic instability.**  

---
## EDA Steps Explained

### Step 1: Import Libraries

Used libraries:
- `pandas`, `numpy` for data manipulation
- `matplotlib`, `seaborn` for visualization
- `sklearn.impute` for handling missing values

---

### Step 2: Load the Dataset

Loaded the Excel file containing happiness report data from 2011 to 2024.

---

### Step 3: Dataset Overview

- Displayed top rows and column data types
- Checked for missing values

**Insights:**
- Key features are numerical
- Some missing data present

---

### Step 4: Data Cleaning

- Simplified and standardized column names
- Removed duplicates

**Result:** Cleaner and more readable data

---

### Step 5: Handle Missing Data

- Visualized missing values using a bar plot
- Imputed numeric columns using the **median**
- Filled missing categorical values with `'Unknown'`

**Technique:** `SimpleImputer` from scikit-learn

---

### Step 6: Descriptive Statistics

- Used `.describe()` to view summary statistics

**Findings:**
- Wide range in GDP, life expectancy, and social support
- Potential outliers identified

---

### Step 7: Univariate Analysis

- Plotted histograms and boxplots of individual variables

**Findings:**
- Happiness scores range between 4–7 in most countries
- Outliers found in generosity and corruption data

---

### Step 8: Multivariate Analysis

- Generated a correlation heatmap
- Explored scatter plots between happiness and key factors

**Correlated Features:**
- GDP per capita 
- Social support 
- Life expectancy 

---

### Step 9: Time Series Analysis

- Tracked average happiness score year by year

**Insight:**
- Global happiness remained stable with slight dips during crises (e.g., COVID-19)

---

### Step 10: Country-Level Insights

- Identified top 10 happiest countries in 2024
- Compared countries like Finland vs Afghanistan

**Top Countries:** Finland, Denmark, Iceland  
**Lowest Countries:** Afghanistan, Lebanon, Zimbabwe

## Key Takeaways & Recommendations

- **Strongest Positive Correlations:** GDP per Capita, Social Support, Healthy Life Expectancy
- **Weaker or Negative Associations:** Freedom, Generosity, Perceptions of Corruption

### Policy Recommendations:
1. **Invest in Health Infrastructure**  
   Countries with higher healthy life expectancy tend to report higher happiness scores.

2. **Improve Economic Opportunities**  
   GDP per Capita is one of the strongest drivers of happiness.

3. **Build Social Support Systems**  
   Social trust and supportive networks significantly influence well-being.

> Policymakers should prioritize **health, economy, and social trust** to improve happiness outcomes.


## Requirements

- Python 3.x
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- openpyxl

Install with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
