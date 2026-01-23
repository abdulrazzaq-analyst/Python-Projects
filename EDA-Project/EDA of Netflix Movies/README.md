# 🎬 Netflix Movies Analysis - Exploratory Data Analysis (EDA)

---

## 📊 Project Overview

---

This project performs a comprehensive exploratory data analysis (EDA) on Netflix's movie catalog, analyzing **16,000 movies** spanning 16 years of content. The analysis examines various dimensions including genres, countries, languages, directors, and financial metrics to understand content trends, audience preferences, and business performance on the streaming platform.

---

## 🎯 Objectives

- Analyze content distribution across genres, countries, and languages
- Identify the most popular and highest-rated movies and categories
- Examine financial performance metrics (budget, revenue, profit)
- Study relationships between budget, popularity, ratings, and revenue
- Identify top-performing directors and countries
- Understand audience engagement patterns and market trends

---

## 📁 Dataset Information

**Data Source:** Kaggle (Netflix Movies Dataset)  
**Records:** 16,000 movies  
**Time Span:** 16 years of content  
**Features:** 18 attributes per movie

### Key Attributes:
- **Basic Information:** Title, Type, Director, Cast, Country, Language
- **Temporal Data:** Date Added, Release Year
- **Content Metrics:** Rating, Duration, Genres, Description
- **Performance Metrics:** Popularity, Vote Count, Vote Average
- **Financial Data:** Budget, Revenue, Profit (calculated)

---

## 🔧 Data Preprocessing

### Data Cleaning Steps:
1. **Missing Values Treatment:**
   - Filled missing director values with 'Unknown' (132 records)
   - Filled missing cast values with 'Unknown' (204 records)
   - Filled missing country values with 'Unknown' (466 records)
   - Filled missing genres values with 'Unknown' (107 records)

2. **Data Optimization:**
   - Dropped unnecessary columns (duration, description)
   - No duplicate records found
   - Added calculated 'profit' column (revenue - budget)

3. **Data Transformation:**
   - Created exploded datasets for genres and countries
   - Grouped data for genre, country, language, and director analysis
   - Applied log scaling for financial distributions

---

## 📈 Key Findings

### Financial Performance:

#### **Top 10 Most Expensive Movies (Budget):**
1. Avatar: The Way of Water - $460M
2. Star Wars: The Rise of Skywalker - $416M
3. Avatar: Fire and Ash - $400M
4. Mission: Impossible - The Final Reckoning - $400M
5. Ant-Man and the Wasp: Quantumania - $388M

#### **Top 10 Highest Revenue Movies:**
1. Avengers: Endgame
2. Avatar: The Way of Water
3. Star Wars: The Force Awakens
4. Avengers: Infinity War
5. Ne Zha 2

#### **Top 10 Most Profitable Movies:**
1. Avengers: Endgame - $2.44B profit
2. Ne Zha 2 - $1.91B profit
3. Avatar: The Way of Water - $1.86B profit
4. Star Wars: The Force Awakens - $1.82B profit
5. Avengers: Infinity War - $1.75B profit

### Content Analysis:

#### **Genre Distribution:**
1. **Drama:** 6,910 movies (most common)
2. **Comedy:** 4,533 movies
3. **Thriller:** 3,769 movies
4. **Action:** 3,239 movies
5. **Romance:** 2,571 movies

#### **Highest Rated Genres:**
1. Animation
2. History
3. War
4. Music
5. Family

#### **Most Popular Genres (Average):**
Top genres by average popularity scores

### Geographical Insights:

#### **Top Content Producing Countries:**
1. **United States:** 6,000+ titles (dominant producer)
2. **Canada:** Significant contributor
3. **France:** Active production hub
4. **United Kingdom:** Major film industry
5. **Belgium, Japan, South Korea:** Notable contributors

#### **Financial Performance by Country:**
- **China:** Highest average budget, revenue, and profit per movie
- **United Kingdom & USA:** Substantial revenue and profit figures
- **India & Australia:** High profitability with moderate budgets
- **Japan, Canada, France:** Consistent revenue generation

#### **Highest Rated Countries:**
1. **Mexico:** Highest average ratings
2. **Greece & Denmark:** Strong European cinema
3. **Brazil & Colombia:** Growing Latin American influence
4. **Japan:** Consistent global appeal

### Language Analysis:

#### **Language Distribution:**
- **English:** 59.6% (dominant language)
- **French:** 6.6%
- **Japanese:** 5.7%
- **Korean:** 5.5%
- **Spanish:** 4.6%
- **Other Languages:** 18.1%

#### **Highest Rated Languages:**
1. **Japanese:** 6.49 average rating
2. **Spanish & Turkish:** Close competitors
3. **All major languages:** Above 6.0 average

#### **Most Profitable Languages:**
1. **Chinese (zh):** $50M+ average profit
2. **English (en):** Significant but lower than Chinese
3. **Hindi (hi) & Japanese (ja):** Good profitability

### Director Analysis:

#### **Most Prolific Directors:**
1. **Tyler Perry:** 20 movies
2. **Sean McNamara, Roel Reine, Steven Soderbergh:** 15 movies each
3. **Other directors:** 13-14 movies

#### **Highest Rated Directors:**
1. **Christopher Nolan**
2. **Denis Villeneuve**
3. **Tosca Musk**
4. **Makoto Shinkai**
5. **Jay Oliva**

#### **Most Profitable Directors:**
1. **Christopher Nolan:** ~$600M average profit per movie
2. **Jon Watts & David Yates:** Major franchise directors
3. **Other blockbuster directors:** High profitability

---

## 📊 Visualizations Created

### Financial Analysis:
1. **Movie Popularity Distribution** - Histogram with KDE
2. **Movie Ratings Distribution** - Histogram with KDE
3. **Budget vs Revenue Distributions** - Log scale histograms
4. **Correlation Heatmap** - Relationships between metrics

### Genre Analysis:
5. **Top Genres by Movie Count** - Horizontal bar chart
6. **Top Genres by Average Rating** - Horizontal bar chart
7. **Top Genres by Average Popularity** - Horizontal bar chart

### Country Analysis:
8. **Top Content Producing Countries** - Horizontal bar chart
9. **Country-wise Budget, Revenue, Profit** - Side-by-side bar charts
10. **Average Rating by Country** - Horizontal bar chart
11. **Average Popularity by Country** - Horizontal bar chart
12. **Movie Release Trends (Top 5 Countries)** - Line chart

### Language Analysis:
13. **Movie Distribution by Language** - Pie chart
14. **Average Rating by Language** - Horizontal bar chart
15. **Average Profit by Language** - Horizontal bar chart

### Director Analysis:
16. **Movies per Director** - Horizontal bar chart
17. **Average Rating by Director** - Horizontal bar chart
18. **Average Profit by Director** - Horizontal bar chart

---

## 🔍 Key Insights

### Content Strategy:
- **Genre Diversity:** Wide variety but dominated by Drama, Comedy, Thriller
- **International Focus:** Strong presence of non-English content (40.4%)
- **Quality vs Quantity:** Most movies have moderate popularity (below 17)
- **Blockbuster Strategy:** Few high-budget movies generate disproportionate revenue

### Financial Patterns:
- **Budget-Revenue Correlation:** Strong positive correlation (0.75)
- **Profit Centers:** China leads in profitability, followed by English markets
- **Efficient Production:** Some countries achieve high profitability with moderate budgets
- **Franchise Power:** Directors involved in major franchises show highest profits

### Geographical Trends:
- **US Dominance:** Leads in content volume and popularity
- **Asian Rise:** Chinese and Japanese content show strong performance
- **European Quality:** Several European countries achieve high ratings
- **Global Distribution:** Content from 1,464 different countries

### Audience Engagement:
- **Rating Patterns:** Most movies rated 5-7/10 (average quality)
- **Popularity Skew:** Few super-hit titles dominate popularity metrics
- **Language Preferences:** English dominance but strong niche language markets
- **Director Influence:** Certain directors consistently deliver high-rated content

---

## 🛠️ Technical Implementation

### Libraries Used:
- **Pandas & NumPy:** Data manipulation and analysis
- **Matplotlib & Seaborn:** Advanced data visualization
- **Jupyter Notebook:** Interactive analysis environment

### Advanced Techniques:
- **Data Explosion:** Handling multi-genre and multi-country entries
- **Log Scaling:** For financial metric distributions
- **Correlation Analysis:** Heatmap for metric relationships
- **Custom Formatters:** Million-formatter for axis labels
- **Theme Customization:** Netflix-inspired dark theme with red accents

### Analysis Methodology:
- **Multi-dimensional Grouping:** By genre, country, language, director
- **Financial Metric Calculation:** Profit analysis and comparisons
- **Trend Analysis:** Temporal patterns in content release
- **Comparative Analysis:** Country-to-country and genre-to-genre comparisons
- **Statistical Summaries:** Averages, distributions, correlations

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
Data Source: Kaggle (Netflix Movies Dataset)
Analysis Period: 16 years of movie data
Tools Used: Python, Pandas, Matplotlib, Seaborn
Purpose: Entertainment Industry Analysis and Insights Generation

---

**Note:** This analysis provides insights into Netflix's content strategy and performance patterns. The findings can inform content acquisition, production decisions, and market strategy in the streaming industry.
