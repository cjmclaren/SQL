# This code utilizes the following Superstore data:

CREATE TABLE superstore (
    item_id INTEGER PRIMARY KEY,
    item_name TEXT,
    category TEXT,
    price DECIMAL(10, 2),
    stock_quantity INTEGER,
    average_rating DECIMAL(3, 2)
);

INSERT INTO superstore (item_id, item_name, category, price, stock_quantity, average_rating)
VALUES
    (1, 'Stainless Steel Cookware Set', 'Kitchen Supplies', 89.99, 50, 4.6),
    (2, 'Memory Foam Mattress', 'Furnishings', 499.99, 30, 4.8),
    (3, 'Smart LED TV', 'Electronics', 549.00, 20, 4.5),
    (4, 'Robot Vacuum Cleaner', 'Appliances', 199.50, 40, 4.3),
    (5, 'Wireless Bluetooth Speaker', 'Electronics', 39.99, 60, 4.2),
    (6, 'Non-Stick Baking Set', 'Kitchen Supplies', 29.95, 80, 4.4),
    (7, 'Cotton Bedding Set', 'Furnishings', 89.00, 25, 4.7),
    (8, 'Smart Home Security Camera', 'Electronics', 79.95, 15, 4.1),
    (9, 'Air Purifier', 'Appliances', 129.50, 35, 4.6),
    (10, 'Premium Coffee Maker', 'Kitchen Supplies', 79.99, 50, 4.9),
    (11, 'Ergonomic Office Chair', 'Furnishings', 189.00, 20, 4.5),
    (12, 'Wireless Earbuds', 'Electronics', 49.99, 75, 4.3),
    (13, 'Slow Cooker', 'Appliances', 49.95, 30, 4.7),
    (14, 'Cutlery Set', 'Kitchen Supplies', 34.50, 40, 4.4),
    (15, 'Cozy Throw Blanket', 'Furnishings', 24.99, 100, 4.2);


#Use a SELECT statement to order items by price from highest to lowest.
SELECT item_name, price
FROM superstore
ORDER BY price desc;

#Show a statistic about prices.
SELECT SUM(price)
FROM superstore;

SELECT AVG(price)
FROM superstore;

SELECT MAX(price)
FROM superstore;

SELECT MIN(price)
FROM superstore;

SELECT COUNT(price)
FROM superstore;

#Show a statistic about prices for items in the Kitchen Supplies category.
SELECT AVG(price)
FROM superstore
WHERE category='Kitchen Supplies';

#How many item names are in each category?
SELECT COUNT(item_name), category
FROM superstore
GROUP BY category;

#How many blankets are in stock?
SELECT stock_quantity
FROM superstore
WHERE item_name='Cozy Throw Blanket';

#How much do Wireless Earbuds cost?
SELECT price
FROM superstore
WHERE item_name='Wireless Earbuds';
