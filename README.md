# 📊 Social Media, Mental Health & Lifestyle Analysis

---

## 📌 Project Overview

This project explores the relationship between social media usage, stress levels, mental health scores, and sleep patterns.  
The analysis is performed using Python data visualization libraries to uncover patterns and insights across different platforms, genders, and age groups.

---

## 🎯 Objectives

- Analyze how different social media platforms relate to stress levels  
- Study gender-wise stress distribution  
- Understand how sleep duration varies with mental health score  
- Explore age-wise relationships between stress and sleep  
- Perform data analysis using Python  

---

## 📂 Dataset Features

- **Gender** – Gender of the user  
- **Age** – Age of the user  
- **Most_Used_Platform** – Primary social media platform  
- **Stress_Level** – Self-reported stress level (Low, Medium, High, Very High)  
- **Mental_Health_Score** – Numerical mental health score  
- **Sleep_Hours_Per_Night** – Average sleep duration per night  

---

## 🛠️ Tools & Libraries Used

- Python  
- Pandas  
- Matplotlib  
- Seaborn  

---

## 📊 Key Analyses Performed

### 1. Stress Level Distribution by Social Media Platform

- Compared stress levels across platforms like WhatsApp, Instagram, Facebook, etc.  
- Used stacked bar charts (100% normalized)

📌 Insight:
- Some platforms show higher proportion of "Very High" stress users  
- Stress distribution varies significantly across platforms  

---

### 2. Gender-wise Stress Analysis

- Visualized stress distribution across genders using stacked bar charts  

📌 Insight:
- Stress levels vary between genders  
- Patterns depend on dataset distribution  

---

### 3. Sleep vs Mental Health Score

- Used regression plot to analyze relationship  

📌 Insight:
- A relationship exists between mental health score and sleep duration  
- Trend line shows correlation direction  

---

### 4. Age vs Stress Level vs Sleep (Heatmap)

- Used heatmap to analyze average sleep hours across age groups and stress levels  

📌 Insight:
- Sleep duration varies with both age and stress level  
- Heatmap provides clearer insights than simple plots  

---


### 5. Country wise most used platform (Heatmap)

- Used heatmap to analyze country wise most used platform
  
📌 Insight:
- India was using platforms like linkedin , instagram and snapchat at a medium rate as compared to other countries 
- Heatmap provides clearer insights than simple plots

---

### 6. Age and academic level wise stress level (Heatmap)

- Used heatmap to analyze stress level among the age and academic level
  
📌 Insight:
- High school students aged 18 were the most stressed among any others 
- 19 years old Undergraduates were the second most high stressed students after the High School students 

---

### 7. Academic level wise Count of Daily Unlocks (Lineplot)

- Used Lineplot to analyze daily unlcoks of students according to their academic level
  
📌 Insight:
- High school students were having the most daily unlocks among any others 
- Graduates were having the least daily unlocks  

---
## 📈 Important Visualizations Used

- 📊 Stacked Bar Charts → Categorical comparisons  
- 📉 Regression Plot → Correlation analysis  
- 🔥 Heatmaps → Multi-variable relationships  
- 📋 Crosstabs → Percentage-based distributions  

---

## ⚠️ Key Learnings

- Stress levels are **ordinal categorical data**, not continuous values  
- Boxplots can be misleading for categorical variables  

### Always define category order:

["Low", "Medium", "High", "Very High"]
Use:
✔ Stacked bar charts for category comparison
✔ Heatmaps for multi-variable relationships

---


📌 Example Code Snippets
Stacked Bar Chart (Stress by Platform)
pd.crosstab(df['Most_Used_Platform'], df['Stress_Level'], normalize='index').plot(kind='bar', stacked=True)
Regression Plot (Sleep vs Mental Health)
sns.regplot(data=df, x="Mental_Health_Score", y="Sleep_Hours_Per_Night")
Heatmap (Age vs Stress vs Sleep)
sns.heatmap(crosstab_data, annot=True, cmap="viridis")
sns.lineplot(data=st_du_mup,y=df["Daily_Unlocks"],x=df["Academic_Level"])

📊 Final Conclusion

The analysis shows that:

Social media platforms are associated with different stress distributions
WhatsApp users showed higher proportions of high stress in this dataset
Sleep duration is moderately related to mental health scores
Age and stress level together influence sleep patterns

---

👨‍💻 Author

Krishna Pandey 
Data Analysis Project | Python EDA


