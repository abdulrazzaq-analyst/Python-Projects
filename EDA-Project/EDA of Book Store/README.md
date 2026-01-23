# 📚 Book Store Sales Analysis - Exploratory Data Analysis (EDA)

---

## 📊 Project Overview

This project performs a comprehensive exploratory data analysis (EDA) on a book store dataset containing **1,070 book records** with 15 different attributes. The analysis focuses on understanding sales patterns, identifying popular genres and publishers, and examining the relationship between book ratings and sales performance.

---

## 🎯 Objectives

- Analyze sales performance across different years, genres, and languages
- Identify top-performing publishers and authors
- Examine the relationship between book ratings and sales
- Explore publishing trends and market patterns
- Provide actionable insights for bookstore management

---

## 📁 Dataset Information

**Dataset:** Books_Data.csv  
**Records:** 1,070 books  
**Columns:** 15 attributes  
**Time Period:** Books published from 1900-2016

### Key Columns:
- Publishing Year, Book Name, Author
- Language, Genre, Publisher
- Book Ratings (Average and Count)
- Sales Metrics (Units Sold, Gross Sales, Revenue)
- Sales Rank and Sale Price

---

## 🔧 Data Preprocessing

### Data Cleaning Steps:
1. **Missing Values Handling:**
   - Removed 23 rows with missing book names
   - Filled 53 missing language codes with 'Unknown'
   - Filtered out invalid publishing years (<1900)

2. **Data Transformation:**
   - Converted publishing year to integer
   - Standardized genre categories (merged 'genre fiction' with 'fiction')
   - Capitalized genre names for consistency

3. **Data Quality Checks:**
   - No duplicate records found
   - All data types appropriately assigned
   - Numerical ranges validated

---

## 📈 Key Findings

### 1. 📅 Publishing Trends
- **Peak Publishing Years:** 2011, 2008, 2012, 2015, 2006
- **Modern Dominance:** Most books published after year 2000
- **Historical Gap:** Very few books published in early 1900s

### 2. 📚 Genre Distribution
- **Fiction Dominance:** Over 80% of published books
- **Nonfiction:** Approximately 10% of total
- **Children's Books:** Minimal representation in dataset

### 3. 🏆 Top Performers

**Top-Selling Authors:**
1. Harper Lee (5,500 units, $47,795)
2. Stephen King (278,322 units, $43,323)
3. David Sedaris (15,193 units, $42,323)

**Most Expensive Books:**
1. The Wind in the Willows - $33.86
2. We Need to Talk About Kevin - $25.89
3. Sabriel - $19.98

**Highest-Rated Books:**
1. Words of Radiance (4.77/5)
2. A Court of Mist and Fury (4.72/5)
3. The Essential Calvin and Hobbes (4.65/5)

### 4. 🏢 Publisher Analysis
- **Market Leader:** Amazon Digital Services, Inc. (highest units sold)
- **Strong Competitors:** Random House LLC, Penguin Group (USA) LLC
- **Revenue Leader:** Penguin Group (USA) LLC (highest publisher revenue)

### 5. 🌍 Language Analysis
- **Primary Language:** English (68% of books)
- **Sub-variants:** eng and en-US dominate sales
- **Other Languages:** Minimal market presence

### 6. ⭐ Rating Analysis
- **Average Ratings:** Most books rated between 3.8 and 4.2
- **Rating-Sales Correlation:** No significant relationship found
- **Author Ratings:** Intermediate-rated authors produce most books

---
## 📊 Visualizations Created

The analysis includes 12 comprehensive visualizations:

1. **Distribution of Publishing Year** (Histogram with KDE)
2. **Percentage of Books by Language** (Pie Chart)
3. **Number of Books in Each Genre** (Bar Chart)
4. **Books Published by Each Publisher** (Horizontal Bar Chart)
5. **Books by Author Rating** (Bar Chart)
6. **Distribution of Book Average Ratings** (Histogram with KDE)
7. **Units Sold by Language** (Bar Chart with million formatting)
8. **Sales Trend Over Years** (Line Chart with markers)
9. **Units Sold by Publisher** (Horizontal Bar Chart)
10. **Units Sold by Author Rating** (Bar Chart)
11. **Total Sales by Genre** (Bar Chart)
12. **Rating vs Units Sold** (Scatter Plot with Regression)
13. **Revenue by Publisher and Genre** (Grouped Bar Chart)

---

## 🔍 Key Insights

### Sales Patterns:
- Sales remained steady until 1990s, then showed significant growth
- Fiction generates highest gross sales, followed by nonfiction
- Amazon dominates unit sales, while Penguin leads in revenue generation

### Market Dynamics:
- No correlation between book ratings and sales volume
- Intermediate and excellent-rated authors dominate market share
- English language books control majority of sales

### Publisher Strategy:
- Amazon's volume strategy vs. Penguin's revenue focus
- Niche publishers (like HarperCollins Christian) have limited market share
- Digital services showing strong growth potential

---

## 🛠️ Technical Implementation

### Libraries Used:
- **Pandas & NumPy** - Data manipulation and analysis
- **Matplotlib & Seaborn** - Data visualization
- **Jupyter Notebook** - Interactive analysis environment

### Analysis Techniques:
- Descriptive statistics and data profiling
- Correlation analysis and hypothesis testing
- Time series analysis for sales trends
- Categorical data analysis for genres and languages
- Grouped aggregations for publisher and author performance

### Code Features:
- Automated million-formatter for large numbers
- Custom theme settings for consistent visualizations
- Dynamic grouping and sorting for rankings
- Comprehensive error handling and data validation

---

## 📝 Conclusion

### Business Recommendations:
1. **Focus on Fiction**: Allocate more resources to fiction category due to market dominance
2. **Publisher Partnerships**: Strengthen relationships with Amazon, Random House, and Penguin
3. **Language Strategy**: Maintain English focus while exploring niche language markets
4. **Rating Neutral Strategy**: Don't over-emphasize ratings in marketing; focus on other factors
5. **Author Development**: Support intermediate authors who show market potential

### Limitations:
- Dataset limited to 1,070 books
- Historical data sparse for early 1900s
- Limited language diversity in dataset
- Potential sampling bias in book selection

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

