# Telecom_Customer_Churn_Analysis

## Overview 📊✨  
This case study dives into customer churn for Databel using Tableau. The goal was to understand why customers leave, identify key churn drivers, and provide actionable insights via interactive dashboards. This project blends data cleaning, exploratory analysis, and dynamic visualizations to support data-driven decisions.

You can access the Visualization here: https://public.tableau.com/app/profile/shalin.sanjay.gund/viz/Book1_17421616331590/Story1 

## Business Questions & Challenges 🤔💡

### Business Questions ❓  
- **What’s the overall churn rate?**  
  👉 Determine the percentage of customers leaving Databel.
- **Who are the high-risk customer segments?**  
  👉 Identify demographics, regions, and service plans most affected.
- **Why are customers churning?**  
  👉 Uncover the key reasons behind customer attrition (e.g., competitor promotions, contract types).
- **How can churn be reduced?**  
  👉 Develop data-backed recommendations to improve retention.

### Challenges & Approach 🚀  
- **Data Quality & Completeness:**  
  The dataset had missing values and duplicates.  
  👉 *Action:* Performed thorough data cleaning and validation for accuracy.
- **Consistent Metric Definition:**  
  Defining churn clearly was crucial.  
  👉 *Action:* Standardized churn rate as the ratio of churned customers to total unique customers.
- **Dynamic Customer Segmentation:**  
  Diverse profiles demanded flexible segmentation techniques.  
  👉 *Action:* Utilized calculated fields, grouping, and parameters in Tableau for interactive analysis.
- **Effective Data Visualization:**  
  Communicating complex insights clearly was a challenge.  
  👉 *Action:* Employed treemaps, dual-axis charts, and maps to illustrate relationships and ensure clarity.

## Tools & Technologies 🛠️🎨  
- **Tableau:** For interactive dashboards and visualizations.  
- **Calculated Fields & Parameters:** To derive key metrics like churn rate and enable dynamic user interaction.  
- **Mapping Tools:** To explore geographical trends in churn.  
- **Data Analysis Techniques:** For detailed segmentation and examination of service usage, contract types, and demographic impacts.

## Analysis Process 🔍📈

### 1. Data Check & Exploration 🧹  
- **Data Cleaning:**  
  Removed duplicates and addressed missing values to ensure data integrity.
- **Initial Exploration:**  
  Developed basic visualizations to understand the dataset's structure.
- **Key Metric Setup:**  
  - **Churn Rate Formula:**
    Churn Rate = (Number of Churned Customers / Total Unique Customers) * 100
  Verified each record represented a unique customer using count and distinct count functions.

### 2. Exploratory Analysis 📊  
- **Calculated Fields:**  
  Created a binomial field for churn using:  
  `IF [Churn Label] == 'No' THEN 0 ELSE 1 END`
- **Churn Categories:**  
  Used treemaps and bubble charts to compare customer counts across churn reasons, revealing competitor promotions as the primary driver.
- **Geographical Insights:**  
  Mapped state-level churn rates, highlighting that California exhibited an exceptionally high churn rate (>60%) 📍.

### 3. Investigating Churn Patterns 🔍  
- **Demographic Analysis:**  
  Senior citizens experienced a churn rate ~10% higher than average.
- **Group Contracts Evaluation:**  
  Analyzed group contracts (multiple customers per household) and found:  
  - Lower average monthly charges are linked to group contracts.  
  - Churn rates are significantly lower compared to individual customers.  
  Dual-axis charts and an interactive parameter (“Pick a Metric”) allowed switching between metrics like number of customers, average monthly charge, churned customers, and customer service calls.
- **Unlimited Data Plan Impact:**  
  Customers on unlimited data plans with low usage (less than 5 GB/month) were more likely to churn.
- **International Call Activity:**  
  Identified that customers purchasing international call plans but using them minimally had higher churn.
- **Contract Type & Payment Methods:**  
  Month-to-month contracts were strongly linked to churn, with a large share of churners falling in this category.

### 4. Dashboarding & Communication 💻🗣️  
- **Overview Dashboard:**  
  Integrated KPIs like total customers, churn rate, and churn reasons into a cohesive dashboard.
- **Interactive Storytelling:**  
  Designed dashboards to be interactive, allowing stakeholders to drill down into specific metrics and intuitively understand the analysis.
- **Effective Communication:**  
  Combined visual insights with narrative elements to make complex findings accessible and actionable.

## Key Insights & Recommendations 🚀📌

- **Overall Churn Rate:**  
  Databel’s churn rate is ~27%—a significant concern.
- **Primary Churn Drivers:**  
  - Competitor promotions contribute ~45% to churn.  
  - Month-to-month contracts are a major factor in attrition.
- **High-Risk Segments:**  
  Senior citizens and customers on unlimited data plans with low usage are particularly vulnerable.
- **Geographical Concerns:**  
  California stands out with an unusually high churn rate, indicating localized challenges.
- **Actionable Recommendations:**  
  - **Targeted Retention:** Develop personalized campaigns for high-risk segments.  
  - **Contract Reevaluation:** Consider revising month-to-month contracts to improve retention.  
  - **Plan Optimization:** Reassess unlimited data plans for low-usage customers to better match needs.  
  - **Enhanced Customer Service:** Focus on areas with high churn rates to better serve vulnerable segments.

## Conclusion 🎯  
This project showcases a systematic approach to analyzing customer churn using Tableau. Through careful data cleaning, insightful exploratory analysis, and dynamic visualizations, key drivers of churn were identified and actionable recommendations provided. This analysis demonstrates technical prowess and the ability to translate data into strategic business solutions.

Feel free to reach out for further details or discussions! 😊👍
