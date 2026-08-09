# 📱 Play Store Data Analysis Dashboard

## 📊 Project Overview

This project presents an interactive **Power BI dashboard for Google Play Store data analysis**. The dashboard is designed to understand app-market trends across categories, installations, ratings, pricing, reviews, and advertising support.

The dashboard provides a high-level business view of the Play Store ecosystem and allows users to explore the data using the **Category slicer** on the left side.

---

## 🎯 Project Objectives

The main objectives of this analysis are to:

- Understand the overall size of the Play Store app market.
- Analyze the distribution of **Free vs Paid apps** based on installs.
- Evaluate the overall **average app rating**.
- Understand the relationship between **ratings and installations**.
- Examine app pricing patterns.
- Analyze the number of apps supporting advertisements and in-app purchases.
- Compare app performance across different categories.
- Build an interactive dashboard that can support data-driven decisions.

---

## 🗂️ Dashboard Structure

The dashboard contains:

1. **Category Filter**
2. **KPI Cards**
3. **Install Distribution by App Type**
4. **Average Rating Gauge**
5. **Price Analysis**
6. **Installations by Rating**
7. **In-App Purchases by Ad Support**

---

## 🔢 Key Performance Indicators

The dashboard currently displays the following overall metrics:

| KPI | Value | Interpretation |
|---|---:|---|
| Total Apps | **11.5K** | Approximate number of apps in the analyzed dataset |
| Total Reviews | **98M** | Total reviews recorded across the apps |
| Total Categories | **36** | Number of app categories represented |
| Total Installs | **4B** | Approximate total installations |
| Average Price | **$0.22** | Average price across the analyzed apps |
| Average Rating | **4.08** | Overall average app rating |

> **Note:** KPI values are displayed in abbreviated form in the dashboard, so the exact underlying values may be slightly different.

---

## 📈 Dashboard Insights

### 1. Free vs Paid App Installs

The **Sum of Installs by Type** chart shows:

- **Free apps:** approximately **3B installs (86.56%)**
- **Paid apps:** approximately **1B installs (13.44%)**

### Insight

Free applications clearly dominate the Play Store in terms of total installations. This suggests that users are much more likely to download apps without an upfront purchase price.

For app developers, a **freemium or advertising-supported business model** may therefore provide a larger potential user base than relying only on upfront paid downloads.

---

### 2. Average Rating

The dashboard reports an overall **average rating of 4.08**.

### Insight

An average rating above 4 indicates generally positive user feedback across the analyzed apps. However, the average rating should be interpreted together with the number of reviews because an app with a small number of reviews may have a high rating but relatively weak evidence of broad user satisfaction.

---

### 3. Installs by Rating

The **Sum of Installs by Rating** line chart compares total installations across different rating values.

The chart indicates that installation volume is not distributed evenly across ratings. There are noticeable peaks around ratings in the **3.5–3.7** and **4.4–4.6** ranges.

### Insight

High installation volume does not necessarily mean that the highest-rated apps receive all downloads. App popularity can also be influenced by factors such as:

- Brand recognition
- App category
- Marketing
- App availability
- App age
- User demand
- Free/paid status

Therefore, rating alone should not be treated as the only predictor of app success.

---

### 4. Price Analysis

The **Count of Category by Price** visual shows the distribution of category records against price values.

The dashboard's average app price is approximately **$0.22**.

### Insight

The relatively low average price suggests that most apps are either free or have a low upfront price.

> **Important:** The current price visual should be reviewed before using it for detailed business conclusions. A count of categories by price is not the same as a direct distribution of app prices. A histogram or column chart showing **number of apps by price range** would provide a clearer price analysis.

---

### 5. Advertising Support and In-App Purchases

The **Count of In-App Purchases by Ad Supported** chart compares apps that support advertisements with apps that do not.

The dashboard shows approximately:

- **Ad Supported = Yes:** ~9K records
- **Ad Supported = No:** ~3K records

### Insight

A large proportion of the analyzed apps are associated with advertising-supported monetization.

This supports the observation from the Free vs Paid analysis: many apps appear to use **free access combined with advertising and/or in-app monetization** rather than relying only on upfront purchase revenue.

---

## 🎛️ Interactivity

### Category Slicer

The left-hand **Category** slicer allows the dashboard user to select:

- Individual app categories
- Multiple categories
- All categories

When a category is selected, the dashboard can be used to examine how the KPIs and visualizations change for that category.

This makes the dashboard useful for category-level comparisons and exploratory analysis.

---

## 💡 Business Questions Answered

This dashboard can help answer questions such as:

1. How many apps are present in the dataset?
2. How many total installs do these apps have?
3. What is the average app rating?
4. Are free or paid apps more popular?
5. Which rating ranges receive the most installations?
6. What is the average app price?
7. How common are advertising-supported apps?
8. How do different categories compare?
9. Does a category have unusually high installations or reviews?
10. How does the app monetization model vary across categories?

---

## 📌 Important Findings

Based on the dashboard:

- **Free apps dominate installations**, accounting for about **86.56%** of total installs.
- The dataset contains approximately **11.5K apps**.
- The dataset contains approximately **98M reviews**.
- There are **36 app categories**.
- Total installations are approximately **4B**.
- The overall average rating is **4.08**.
- The average app price is approximately **$0.22**.
- A large number of apps are associated with **advertising support**.
- App rating and app popularity are not necessarily directly proportional.

---

## ⚠️ Data Visualization Considerations

A few visuals could be improved for stronger analytical interpretation:

### Price Visualization

Instead of **Count of Category by Price**, consider using:

- Number of apps by price range
- Average price by category
- Free vs Paid apps by category
- Median price by category

Example price buckets:

```text
Free
$0.01–$1
$1–$5
$5–$10
$10+
```

### Rating Visualization

For rating analysis, consider adding:

- Number of apps by rating
- Average installs by rating
- Median installs by rating
- Reviews vs rating scatter plot

### Monetization Analysis

A useful additional visual would be:

**Free/Paid Type × Ad Supported**

This could reveal how different monetization strategies are used together.

---

## 🛠️ Tools & Technologies

- **Power BI** – Dashboard development and visualization
- **Power Query** – Data cleaning and transformation
- **DAX** – Measures and KPI calculations
- **Microsoft Excel / CSV** – Data source and preprocessing
- **Data Visualization** – Interactive charts, slicers, and KPI cards

---

## 📂 Suggested Project Structure

```text
Play-Store-Data-Analysis/
│
├── README.md
├── data/
│   └── google_playstore_2026.csv
│
├── powerbi/
│   └── Play_Store_Data_Analysis.pbix
│
└── screenshots/
    └── dashboard.png
```

---

## 🚀 Recommended Future Analysis

The project can be extended with:

- Top 10 apps by installs
- Top 10 apps by reviews
- Category-wise average rating
- Category-wise total installs
- Free vs Paid app count by category
- Price distribution
- Reviews-to-install ratio
- Rating-to-install relationship
- Ad-supported vs non-ad-supported comparison
- In-app purchase analysis
- Category profitability analysis
- Interactive Top-N filters

---

## 🧠 Conclusion

The Play Store dashboard provides a concise overview of app-market performance using key metrics such as **installs, reviews, ratings, price, category, and monetization features**.

The strongest finding is the dominance of **free apps**, which account for roughly **86.56% of total installations**. The combination of a high average rating (**4.08**) and a large review volume (**98M**) indicates substantial user engagement in the dataset.

The dashboard can be used as a foundation for deeper analysis of **app popularity, user satisfaction, pricing strategy, and monetization models**.

---

## 👤 Project Type

**Data Analytics / Power BI Dashboard Project**

This project demonstrates skills in:

- Data cleaning
- Exploratory data analysis
- Data visualization
- KPI creation
- Power BI dashboard development
- Business insight generation
- Interactive reporting

---

## ⭐ Key Takeaway

> **Free apps attract the majority of installations, while advertising and other monetization mechanisms appear to play an important role in the Play Store app ecosystem.**
