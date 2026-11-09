# E-commerce Sales and User Behavior Analysis

## Task

Analyze sales and user behavior of an online furniture store (349,545 sessions, November 2020 – January 2021): find the main markets, product categories, devices and traffic channels, check sales dynamics and test statistical relationships and differences between user groups.

## What the analysis does

- Extracts and joins six tables from Google BigQuery with SQL into one dataset
- Describes the data and explains missing values (guests, sessions without purchases)
- Ranks countries, continents and product categories by revenue and number of orders
- Shows the sales structure by device, operating system, browser and traffic channel
- Analyzes user registration, verification and subscription status
- Shows revenue dynamics by day, weekday, continent, device, browser, operating system and channel
- Builds pivot tables and heatmaps (countries × categories, devices × channels, browsers × operating systems)
- Tests correlations between sessions and revenue and between groups over time
- Tests differences between groups: registered vs guest users, channels, devices, share of organic and paid traffic by region

## Techniques used

SQL (`JOIN`, `LEFT JOIN`, `CASE WHEN`), Pandas (`groupby`, `agg`, `pivot_table`, `merge`), data visualization with Matplotlib and Seaborn (lollipop and bar charts, donut charts, line charts, heatmaps, scatter plots, pair plots), statistical tests with SciPy and Statsmodels (Shapiro-Wilk, Spearman correlation, Wilcoxon signed-rank test, Kruskal-Wallis test, two-proportion z-test)

## Key findings

- The United States is the largest market (about 14M in revenue); the Americas bring more than twice as much revenue as Asia
- Sofas & armchairs and Chairs are the top categories by revenue
- Most purchases come from desktop (58.7%) and from Organic Search (35.5%) and Paid Search (27.0%)
- Sales are highest on Tuesday and Wednesday and lowest at weekends; revenue peaks in the second half of December
- Daily sessions and revenue have a very strong positive correlation (Spearman ≈ 0.90)
- There is no statistically significant difference in daily revenue per session between registered and guest users

## Dashboard

[Analytics Dashboard on Tableau Public](https://public.tableau.com/app/profile/nastasiia.nelina/viz/AnalyticsDashboard_17930397692660/AnalyticsDashboard)
