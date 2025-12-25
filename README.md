Amazon Product Reviews – Power BI Dashboard
Overview
This project is an end‑to‑end Amazon product reviews analysis built in Power BI.
The dashboard explores how pricing, discounts, ratings, and reviewer behavior interact to influence product performance and customer sentiment.

Dataset
Source: Amazon product and review data (CSV file).

Rows: 1,465 records (each row is a product–review combination).

Key fields:

product_id, product_name, category

actual_price, discounted_price, discount_percentage

rating, rating_count

review_id, review_content, user_id, user_name

Dashboard Pages
1. Product & Review Overview
Main questions: Which products and categories perform best, and how are reviews distributed?

Key visuals:
  Price vs Discounted Price by Product
    Scatter plot showing relationship between actual and discounted price for each product, useful to spot pricing strategies and heavy discounting.
  
  Top 10 Products by Number of Ratings
    Bar chart ranking products by rating_count to highlight the highest‑visibility items.

  Number of Reviews by Rating
    Area/line chart showing how many reviews occur at each star rating (2.0–5.0), with a reference line at rating 4.0 to highlight where reviews cluster.
  
  Top 10 Reviewers by Number of Reviews
    Bar chart identifying “power reviewers” based on the count of review_id per user_id.
  
  Top 10 Category Distribution
    Donut chart showing the share of products in the top categories based on distinct product_id counts.
  
  KPI Cards
    Average Rating
    Total Number of Ratings (sum of rating_count)
    Total Products (distinct product_id)
    Average Discount %

How to Use the Report
  Download the Amazon_Reviews_Dashboard.pbix file from this repository.
  Open it in Power BI Desktop (latest version recommended).
  If the data is not embedded:
    Place the CSV file in the /data folder.
    Update the file path in Power Query if prompted.

  Interact with the dashboard:
    Use slicers (Category, Rating, Price ranges) to filter views.
    Hover over scatter and bar charts for detailed tooltips.
    Drill into specific products or categories to explore underlying patterns.
