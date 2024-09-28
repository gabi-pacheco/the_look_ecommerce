# The Look - E-commerce Website Performance Analysis

## Project Overview

The Look project analyzes the performance of an e-commerce platform using the [Kaggle dataset](https://www.kaggle.com/datasets/mustafakeser4/looker-ecommerce-bigquery-dataset?resource=download&select=inventory_items.csv) by exploring user behavior, conversion rates, drop-off points, and customer journeys. By examining traffic sources and their effectiveness, the goal is to enhance the overall user experience, optimize marketing strategies, and ultimately drive higher conversions.

## Key Business Questions

1. **Which marketing channels drive the highest conversion rate?**  
   We aim to identify which traffic sources convert visitors into buyers most effectively, helping refine marketing efforts.

2. **How do customer segments respond to different marketing channels?**  
   By analyzing customer behavior (e.g., high spenders, repeat customers), we can determine which segments are more responsive to specific channels.

3. **What is the cart abandonment rate, and how does it vary by traffic source and product category?**  
   Understanding abandonment patterns can reveal potential areas of improvement in the purchase journey.

4. **Which marketing channels drive repeat purchases?**  
   Analyzing customer retention by traffic source helps assess the effectiveness of campaigns in building long-term customer relationships.

5. **How long does the average customer take to complete a purchase, and how can we reduce this time?**  
   Optimizing the customer journey by reducing the time between cart addition and purchase can improve the conversion rate.

6. **What are the top-performing product categories in terms of conversion and abandonment rates?**  
   This helps influence inventory planning and promotion strategies.

7. **How can we predict customer churn and reduce cart abandonment?**  
   By identifying early indicators of churn, we can implement strategies to prevent customers from leaving without purchasing.

8. **How does seasonality affect customer behavior and conversion rates?**  
   Analyzing seasonal trends can reveal patterns that inform marketing and inventory decisions during peak times.

## The Dataset

The Look E-commerce Dataset provides a comprehensive view of online retail operations, encompassing various dimensions such as sales transactions, customer information, product attributes, website engagement metrics, logistics, and additional metadata. This dataset serves as a valuable resource for analyzing and understanding the dynamics of e-commerce business activities.

### Tables:

- **events**: This table records various events related to user interactions.

  **Fields**: `id`, `user_id`, `sequence_number`, `session_id`, `created_at`, `ip_address`, `city`

- **order_items**: This table contains information about items included in orders.

  **Fields**: `id`, `order_id`, `user_id`, `product_id`, `inventory_item_id`, `status`, `created_at`, `shipped_at`

- **orders**: This table stores data related to orders placed by users.

  **Fields**: `order_id`, `user_id`, `status`, `gender`, `created_at`, `returned_at`, `shipped_at`, `delivered_at`, `num_of_item`

## Analysis Approach

The analysis is structured around several key metrics and visualizations:

- **Conversion Funnel**  
  Visualize the customer journey from visits to purchases, focusing on different entry points (Home, Department, Product) and tracking drop-off rates at each stage.

- **Conversion Rate by Traffic Source**  
  Analyze how well each marketing channel converts traffic into purchases.

- **Revenue and Average Order Value (AOV) by Traffic Source**  
  Identify which channels generate the most revenue and the average spending per order.

- **Time to Purchase**  
  Calculate the time it takes for a visitor to make a purchase, segmented by entry point and analyzed over time, with outliers capped to present a realistic average.

- **Customer Retention by Traffic Source**  
  Analyze which channels drive repeat purchases and how they perform in retaining customers.

- **Churn Rate**  
  Calculate the churn rate for sessions that add items to the cart but do not result in a purchase.

- **Trend Analysis**  
  Compare year-over-year changes in key metrics, such as the median time to purchase.
