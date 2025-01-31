# Advanced-Sales-Dashboard-in-Tableau
This project showcases a Sales Dashboard built using Tableau, providing key insights into sales performance, product revenue, customer engagement, and discount trends. The dashboard is designed to support data-driven decision-making for sales managers, marketers, and executives.

## Features

- Revenue Analysis: Identify top revenue-generating product categories.

- Customer Engagement: Understand how product ratings correlate with sales.

- Discount Impact: Evaluate how discounts affect revenue.

- Top Performing Products: Highlight the best-selling products.

- Interactive Filters: Dynamic analysis based on category, product, and discount levels.

## Dataset Information

- Source: Amazon product sales data.

- Size: 1,465 records with 16 columns.

- Key Fields: product_id, product_name, category, actual_price, discounted_price, discount_percentage, rating, rating_count, total_revenue.

## Data Processing Steps

### Data Cleaning

- Removed currency symbols.

- Filled missing rating_count values with the median.

- Standardized percentage formats.

### Derived Metrics

- Total Revenue: discounted_price * rating_count

- Discount Amount: actual_price - discounted_price

- Profit Margin: (discounted_price / actual_price) * 100

### Advanced Calculations in Tableau

- Weighted Average Rating: SUM(rating * rating_count) / SUM(rating_count)

- Category Revenue Share: SUM(total_revenue) / TOTAL(SUM(total_revenue)) * 100

## Visualizations

1. Revenue by Category (Bar Chart): Displays revenue distribution across product categories.

2. Top 10 Products by Revenue (Ranked List): Highlights high-revenue products.

3. Ratings vs. Revenue (Scatter Plot): Shows the correlation between customer ratings and revenue.

4. Average Discount by Category (Bar Chart): Analyzes how discount strategies vary across categories.

5. Top 10 Products by Category (Dynamic Table): Displays the best-selling products within each category.

## Interactive Features

- Category & Product Filters: Drill-down analysis by product category.

- Hover Tooltips: Additional insights on sales and customer engagement.

- Sorting & Ranking: Identify top-performing products easily.

## Evaluation and Key Findings

- High-Revenue Categories: Certain categories generate significantly higher revenue.

- Discount Optimization: Higher discounts do not always lead to increased revenue.

- Customer Ratings Impact: Products with higher ratings tend to perform better.

## Recommendations

- Leverage High-Revenue Categories: Focus marketing and inventory strategies on high-performing categories.

- Optimize Discount Strategies: Ensure discounting aligns with revenue impact.

- Improve Customer Engagement: Promote highly rated products and improve low-rated ones.

- Enhance Data with Time-Based Trends: Implement a timestamp to analyze seasonal trends.

## How to Use This Project

- Download the Tableau Workbook (.twb file) and open it in Tableau.

- Interact with Filters to explore category-specific insights.

- Analyze Key Trends in revenue, customer engagement, and discounts.

## Future Enhancements

- Integrate Live Data Feeds for real-time analysis.

- Incorporate Machine Learning Models for predictive sales forecasting.

- Expand Customer Segmentation by including demographic data.
