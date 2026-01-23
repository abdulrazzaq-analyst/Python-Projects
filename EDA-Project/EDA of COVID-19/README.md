# 🌍 COVID-19 Global Impact Analysis - Exploratory Data Analysis (EDA)

---

## 📊 Project Overview

---

This project conducts a comprehensive exploratory data analysis (EDA) of the global COVID-19 pandemic using data from the World Health Organization (WHO). The analysis covers **489,360 daily records** spanning from January 4, 2020, to August 3, 2025, providing insights into the pandemic's progression, regional impacts, and mortality patterns across 240 countries.

## 🎯 Objectives

---

- Analyze global COVID-19 trends and patterns over time
- Identify countries and regions most affected by the pandemic
- Calculate mortality rates and death ratios across different regions
- Compare the impact across WHO regions
- Identify countries with minimal or no reported cases
- Understand the temporal dynamics of the pandemic

## 📁 Dataset Information

---

**Data Source:** World Health Organization (WHO)  
**Time Period:** January 4, 2020 - August 3, 2025  
**Records:** 489,360 daily reports  
**Countries:** 240  
**WHO Regions:** 7  
**Data Points:** 4 years, 7 months of daily data

### Dataset Structure:
- Date_reported: Daily reporting date
- Country: Country name
- WHO_region: WHO regional classification
- New_cases: Daily new COVID-19 cases
- Cumulative_cases: Running total of cases
- New_deaths: Daily new COVID-19 deaths
- Cumulative_deaths: Running total of deaths

---

## 🔧 Data Preprocessing

### 1. **Missing Values Handling:**
   - Filled 279,022 missing New_cases with 0 (indicating no cases reported)
   - Filled 335,385 missing New_deaths with 0 (indicating no deaths reported)
   - Dropped Country_code column (2,039 missing values, redundant due to complete Country column)

### 2. **Data Quality Assurance:**
   - No duplicate records found
   - Negative values in New_cases and New_deaths clipped to 0
   - Data types optimized (datetime conversion, integer casting)

### 3. **Data Transformations:**
   - Created aggregated views by country, region, and date
   - Calculated death ratios for countries and regions
   - Formatted large numbers for visualization clarity

---

## 📈 Key Findings

### **Global Statistics:**
- **Total Reported Cases:** 778,555,963
- **Total Reported Deaths:** 7,066,337
- **Global Death Ratio:** 0.91%

### **Critical Dates:**
- **Peak Cases Day:** January 30, 2022 (8,401,963 cases)
- **Peak Deaths Day:** January 24, 2021 (27,939 deaths)

### **Geographical Insights:**

#### **Most Affected Countries (Cases):**
1. **United States:** Over 100 million cases
2. **China:** Approximately 100 million cases
3. **Other countries:** Below 50 million cases

#### **Most Affected Countries (Deaths):**
1. **United States:** 1.2 million deaths
2. **Brazil:** 700,000 deaths
3. **India:** 500,000+ deaths

#### **Highest Death Ratios (Countries):**
1. **Yemen:** 18.0%
2. **Sudan:** 7.8%
3. **Syrian Arab Republic:** 5.5%+

---

### **Regional Analysis:**

#### **Cases by WHO Region:**
1. **European Region (EUR):** ~280 million cases
2. **Western Pacific Region (WPR):** ~200 million cases
3. **Americas Region (AMR):** ~200 million cases

#### **Deaths by WHO Region:**
1. **Americas Region (AMR):** ~3 million deaths
2. **European Region (EUR):** ~2.2 million deaths
3. **Other regions:** Below 600,000 deaths

#### **Death Ratios by WHO Region:**
1. **African Region (AFR):** Highest death ratio
2. **Americas Region (AMR):** Moderate death ratio
3. **Western Pacific Region (WPR):** Lowest death ratio

### **Pandemic-Free Zones:**
- **No Reported Cases:** Democratic People's Republic of Korea, Turkmenistan
- **No Reported Deaths:** 13 countries including Falkland Islands, Holy See, Niue, Pitcairn Islands, Saint Helena, Tokelau

---

## 📊 Visualizations

### **Time Series Analysis:**
1. **COVID-19 Cases Trend Worldwide:** Line chart showing pandemic waves and peaks
2. **COVID-19 Deaths Trend Worldwide:** Line chart highlighting mortality patterns

### **Geographical Distribution:**
3. **Top 10 Countries by Cases:** Horizontal bar chart
4. **Top 10 Countries by Deaths:** Horizontal bar chart
5. **Highest COVID-19 Death Ratios:** Bar chart for country-level mortality

### **Regional Analysis:**
6. **WHO Region-wise Cases:** Bar chart comparing regions
7. **WHO Region-wise Deaths:** Bar chart with mortality comparison
8. **COVID-19 Death Ratio by WHO Region:** Regional mortality analysis
9. **Cases Distribution by WHO Region:** Pie chart showing regional contributions
10. **Deaths Distribution by WHO Region:** Pie chart with mortality distribution

---

## 🔍 Key Insights

### **Temporal Patterns:**
- Initial slow spread in early 2020 followed by explosive growth
- Major surge in early 2022 with cases exceeding 8 million daily
- Post-2023 stabilization into endemic phase
- Deaths peaked in 2020-2022 then significantly declined

### **Geographical Disparities:**
- Significant inequality in pandemic impact across regions
- Developed countries reported higher absolute numbers but lower death ratios
- Developing regions showed higher mortality rates despite lower case numbers
- Several small island nations and territories avoided the pandemic entirely

### **Regional Characteristics:**
- **Europe:** Highest case burden but moderate mortality
- **Americas:** Highest death burden with significant mortality
- **Africa:** Highest death ratio indicating healthcare challenges
- **Western Pacific:** Effective containment with lowest death ratio

---

## 🛠️ Technical Implementation

### **Libraries Used:**
- **Pandas & NumPy:** Data manipulation and analysis
- **Matplotlib & Seaborn:** Advanced data visualization
- **Jupyter Notebook:** Interactive analysis environment

### **Technical Features:**
- Custom million-formatter for axis labels
- Advanced time series analysis techniques
- Regional grouping and aggregation methods
- Statistical correlation and ratio calculations
- Professional visualization themes and formatting

### **Analysis Methodology:**
- Time series decomposition for trend analysis
- Geographical clustering and regional comparison
- Mortality ratio calculations and benchmarking
- Outlier detection and data validation
- Comparative analysis across multiple dimensions

---

## 🌐 Portfolio Website
Explore more of my data analytics projects:  
👉 https://abdulrazzaq-analyst.github.io/Portfolio_Website/

---

## 📞 Contact
For questions or collaboration:  
📧 abdulrazzaq.analytics@gmail.com  
🔗 https://github.com/abdulrazzaq-analyst

---

## 👤 Author
**Abdul Razzaq**  
Statistics Graduate | Data Analytics & Visualization  
🔗 GitHub: https://github.com/abdulrazzaq-analyst

---

## 📋 Acknowledgments
Data Source: World Health Organization (WHO)
Analysis Period: 2020-2025
Tools Used: Python, Pandas, Matplotlib, Seaborn
Purpose: Educational and Research Analysis
---

**Note:** This analysis is based on officially reported data. Actual infection and mortality rates may vary due to reporting differences and asymptomatic cases. The analysis aims to provide insights into reported trends and patterns for research and learning purposes.
