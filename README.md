# Amazon Sales Analysis Dashboard

## Project Overview

This project is an **Amazon product sales and customer review analysis
dashboard** built using **Microsoft Power BI**. The project uses an
Amazon product dataset containing product details, pricing, discounts,
ratings, rating counts, categories, and customer review information.

The goal is to transform raw Amazon product data into an interactive
dashboard that helps users understand **product performance, pricing,
discounts, ratings, and category-level insights**.

## Project Objectives

-   Analyze Amazon product pricing and discount patterns.
-   Identify product and category-level performance.
-   Understand customer rating distribution.
-   Compare actual prices and discounted prices.
-   Monitor average product ratings and discounts.
-   Provide an interactive dashboard for filtering and exploration.
-   Present business insights in a simple and visual format.

## Dataset

**Dataset:** `amazon.csv`

The dataset contains **1,465 records** and **16 columns**. It includes
product, pricing, category, rating, and customer review information.

### Main Columns

  Column                  Description
  ----------------------- ------------------------------
  `product_id`            Unique product identifier
  `product_name`          Name of the product
  `category`              Product category hierarchy
  `discounted_price`      Product price after discount
  `actual_price`          Original product price
  `discount_percentage`   Percentage discount offered
  `rating`                Customer rating
  `rating_count`          Number of customer ratings
  `about_product`         Product description
  `user_id`               Customer identifier
  `user_name`             Customer name
  `review_id`             Review identifier
  `review_title`          Review title
  `review_content`        Customer review text
  `img_link`              Product image URL
  `product_link`          Amazon product URL

The dataset contains **1,351 unique product IDs** across **9 top-level
product categories**.

## Tools & Technologies

-   **Microsoft Power BI** -- Dashboard development and visualization
-   **Power Query** -- Data cleaning and transformation
-   **DAX** -- Measures and calculations
-   **CSV** -- Source dataset
-   **Data Analysis** -- Product, pricing, discount, and rating analysis

## Data Cleaning & Transformation

The raw dataset was prepared before visualization using Power Query.

Key preparation steps included:

1.  Imported the Amazon CSV dataset into Power BI.
2.  Checked column names and data types.
3.  Converted `discounted_price` and `actual_price` from text/currency
    values into numeric values.
4.  Converted `discount_percentage` into a numeric percentage field.
5.  Converted `rating` into a numeric field.
6.  Converted `rating_count` into a numeric field after removing commas.
7.  Split the hierarchical `category` field into separate category
    levels.
8.  Checked for missing values.
9.  Created calculated measures required for the dashboard.
10. Used the cleaned data to build interactive visualizations.

## Power BI Dashboard

The `.pbit` file contains an interactive dashboard with KPI cards,
charts, a category slicer, and a branded Amazon-style layout.

### Dashboard Components

#### 1. Total Products

Displays the total number of products represented in the dashboard.

#### 2. Average Rating

Shows the overall average customer rating across the products.

#### 3. High Rated Sales

Highlights the sales/value measure associated with highly rated
products.

#### 4. Average Discount Gauge

Displays the average discount percentage and compares it against a
target discount.

#### 5. Sales by Category

A donut chart is used to compare the sales/value contribution of
different top-level product categories.

#### 6. Product Price Comparison

A clustered bar chart compares product IDs based on their
original/actual price values.

#### 7. Rating Distribution

A funnel chart shows the number of products associated with different
customer rating levels.

#### 8. Discount vs Rating Analysis

A scatter chart is used to explore the relationship between product
discounts and ratings.

#### 9. Category Slicer

An interactive hierarchical slicer allows users to filter the dashboard
by product category and subcategory.

## Key Analytical Areas

The dashboard focuses on four major areas:

### Product Performance

-   Number of products
-   High-rated products
-   Product-level price comparison

### Pricing & Discounts

-   Actual price
-   Discounted price
-   Discount percentage
-   Average discount
-   Discount target comparison

### Customer Feedback

-   Average rating
-   Rating distribution
-   Rating counts
-   Review-related product information

### Category Analysis

-   Sales/value by category
-   Category filtering
-   Subcategory exploration
-   Comparison between major Amazon product groups

## Sample Dataset Insights

After basic data cleaning:

-   **1,465** dataset records
-   **1,351** unique product IDs
-   **9** top-level categories
-   Average rating: approximately **4.10 / 5**
-   Average listed discount: approximately **47.69%**

The dashboard should be used for visual exploration rather than treating
the dataset as a transactional sales ledger, because the source data
primarily contains product and review information.

## Project Files

``` text
Amazon-Sales-Analysis/
│
├── README.md
├── amazon.csv
└── Amazon sales.pbit
```

### File Description

-   `README.md` -- Project documentation
-   `amazon.csv` -- Raw Amazon product/review dataset
-   `Amazon sales.pbit` -- Power BI dashboard template

## How to Use the Project

1.  Download or clone the project repository.
2.  Open `Amazon sales.pbit` using **Microsoft Power BI Desktop**.
3.  When prompted, connect the report to `amazon.csv`.
4.  Verify the data source path.
5.  Refresh the dataset.
6.  Use the category slicer to explore different product groups.
7.  Interact with the charts to analyze pricing, discounts, ratings, and
    category performance.

## Business Questions Answered

This dashboard can help answer questions such as:

-   How many products are available in the dataset?
-   Which product categories have the highest sales/value contribution?
-   What is the average customer rating?
-   What is the average discount offered?
-   How are products distributed across rating levels?
-   Which products have higher original prices?
-   Is there an observable relationship between discount levels and
    ratings?
-   How does product performance change when different categories are
    selected?

## Skills Demonstrated

This project demonstrates practical skills in:

-   Data cleaning
-   Data transformation
-   Power Query
-   Data modeling
-   DAX measures
-   KPI development
-   Interactive dashboard design
-   Data visualization
-   Business analysis
-   Customer review analysis
-   Pricing and discount analysis

## Future Improvements

Possible improvements include:

-   Add time-based sales analysis if transaction-date data becomes
    available.
-   Add top 10 products by sales/value.
-   Add top products by rating and review count.
-   Add discount impact analysis.
-   Add customer sentiment analysis using review text.
-   Add drill-through product detail pages.
-   Add more advanced DAX measures.
-   Add a dedicated executive summary page.

## Author

**Rakesh Jami**

### Project Type

**Power BI Data Analytics Project -- Amazon Sales & Product Analysis**
