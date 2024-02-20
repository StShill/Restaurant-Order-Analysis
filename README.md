# SQL DATA EXPLORATION Restaurant-Order-Analysis

## Project Overview


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
- 

### Data Source
- Maven Ananlytics
  
### Data Tools
- MYSQL

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


### Data Insights
