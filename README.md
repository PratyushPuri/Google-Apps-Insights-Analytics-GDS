# Google Play Store Market Intelligence Dashboard

<div align="center">

<img src="https://static0.anpoimages.com/wordpress/wp-content/uploads/2022/06/what-is-google-play-hero.jpg" alt="drawing" width="500"/>

</div>

## Overview
Interactive Looker Studio dashboard analyzing 10.3K cleaned Google Play Store apps, providing real-time insights on ratings, installs, category performance, and market trends. Empowers stakeholders to make data-driven decisions for app development and marketing strategies.

## Dataset Overview
- **Size**: 10,300 apps after data cleaning from the original Google Play Store dataset, removing duplicates and handling missing values.
- **Source**: Cleaned dataset (`cleaned_googleplaystore.csv`) generated from `google-play-store-analytics.ipynb` through comprehensive data preprocessing.
- **Key Metrics**: Average rating of 4.2 across all apps, 92.6% free apps, average installs of 14.2 million per app.
- **Categories**: 33 app categories with GAME leading at 21.51% of total installs, followed by COMMUNICATION (8.53%) and SOCIAL (8.53%).
- **Install Segments**: Categorized into Very High (>1M installs with 4,059 apps), High (100K-1M with 1,645 apps), Medium (1K-100K), and Low (<1K).
- **Rating Distribution**: Segmented into Excellent (4.5-5), Very Good (4-4.5), Good (3-4), Fair (2-3), and Poor (≤2) for granular performance tracking.
- **Time Period**: Apps tracked from 2010-2018 showing evolution and update patterns across different years.

## Analysis & Dashboard
- **Data Preprocessing**:  
  - Cleaned raw dataset using Python in Jupyter notebook, handling missing ratings, converting size and install formats to numeric values, removing duplicates.
  - Exported cleaned data to `cleaned_googleplaystore.csv` for dashboard integration, ensuring data quality and consistency for visualization.
  - Standardized category names, price formats, and date fields to enable accurate filtering and aggregation in Looker Studio.

- **Dashboard Components**:  
  - Created KPI cards showing total apps (10.3K), average ratings (4.2), free app percentage (92.6%), and average installs (14.2M) for quick executive overview.
  - Built category distribution pie chart revealing FAMILY (43%), GAME (18.7%), TOOLS (8.1%) as dominant categories by app count.
  - Designed install performance table segmenting apps by install ranges (1M+, 500K+, 100K+) with corresponding app counts and ratings for performance benchmarking.
  - Developed treemap visualization showing average installs per category, highlighting GAME's 21.51% share and COMMUNICATION's 8.53% contribution to total installs.

- **Interactive Features**:  
  - Added category and type filters enabling stakeholders to drill down into specific app segments and explore free vs paid app dynamics.
  - Implemented rating distribution stacked bar chart showing performance across install segments, revealing that Very High install apps have 44.19% in Very Good ratings.
  - Created time-series analysis of record count distribution by rating from 2010-2018, tracking rating quality evolution and identifying 2017-2018 as peak update periods.

- **Insights Delivered**:  
  - GAME category dominates both app count and install share, validating continued investment in gaming app development.
  - Higher install segments correlate with better rating distributions, with Very High segment showing 35.75% Excellent ratings versus 5.08% for Low segment.
  - Free apps constitute 92.6% of the market, confirming freemium as the dominant business model requiring focus on in-app monetization strategies.
  - Rating quality has improved over time with newer apps (2016-2018) showing higher proportions of Good and Very Good ratings compared to earlier years.

## How to Use
- Access the live dashboard:  
  [Google Play Store Market Intelligence Dashboard](https://lookerstudio.google.com/u/0/reporting/6f019c6e-343d-40f3-b97f-4c352c0ac963)
- Use the interactive filters:  
  - Select **Category** dropdown to analyze specific app categories (GAME, COMMUNICATION, SOCIAL, etc.)
  - Toggle **Type** filter to compare Free vs Paid app performance metrics
  - Click on chart elements to cross-filter and explore relationships between metrics
- Navigate dashboard sections:  
  - Top KPI row provides high-level market overview
  - Category Distribution pie chart shows market composition
  - Install Performance Table ranks apps by install segments
  - Rating Distribution chart analyzes quality across install brackets
  - Time-series chart tracks rating evolution from 2010-2018
- For data updates:  
  - Run `google-play-store-analytics.ipynb` with new raw data
  - Generate updated `cleaned_googleplaystore.csv` file
  - Upload to Looker Studio data source to refresh dashboard automatically
- Export insights:  
  - Download charts as images for presentations
  - Export filtered data tables to CSV for further analysis
  - Share dashboard link with stakeholders for collaborative decision-making
- Best practices:  
  - Start with category filter to focus on your target market segment
  - Compare Free vs Paid performance to inform pricing strategies
  - Monitor rating distribution to identify quality benchmarks
  - Track time trends to understand market evolution and competitive landscape

## Author & Contact
- Name: `Pratyush Puri`  
- Contact: `pratyushpuri17@gmail.com`  
- LinkedIn: [https://www.linkedin.com/in/pratyushpuri](https://www.linkedin.com/in/pratyushpuri)
