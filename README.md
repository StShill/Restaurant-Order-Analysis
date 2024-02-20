# SQL DATA EXPLORATION Restaurant-Operations-Analysis

## Project Overview
In this project I use my analytic tools to explore a restaurant operations by digging into the customer data to see which menu items are doing well/not well and what the top customers seem to like best. 
I explore both tables to understand how customers are reacting to the new menu based off the data I have queried

### Queries Used
- SELECT 
- FROM 
- COUNT
- ASC
- DESC
- WHERE
- ORDER BY
- GROUP BY
- ALIAS


### Data Source
- Maven Ananlytics
  
### Data Tools
- MYSQL
### SQL Tables
- menu_items
- order_details
### Data Exploration 
1. Find the number of items on the menu?
   
-  SELECT COUNT(*) FROM menu_items;
  
2. What are the least and most expensive items on the menu?

- SELECT * FROM menu_items
ORDER BY price ASC;

- SELECT * FROM menu_items
ORDER BY price DESC;

3. How many italian dishes are on the menu?

- SELECT COUNT(*) FROM menu_items
WHERE category = 'italian';

4. What are the least and most expensive italian dishes on the menu? 

- SELECT * FROM menu_items
WHERE category = 'italian'
ORDER BY price ASC;

- SELECT * FROM menu_items
WHERE category = 'italian'
ORDER BY price DESC;


5. How many dishes are in each category?

- SELECT category, COUNT(menu_item_id) AS num_dish
FROM menu_items
GROUP BY category;
  
6. What is the average dish price within each category?
   
- SELECT category, Avg(price) AS avg_price
FROM menu_items
GROUP BY category;

### Data Insights
