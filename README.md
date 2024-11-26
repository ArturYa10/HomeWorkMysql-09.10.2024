# HomeWorkMysql-09.10.2024

CREATE TABLE goods (
    id SERIAL PRIMARY KEY,
    title VARCHAR(255),
    quantity INTEGER
);


INSERT INTO goods (title, quantity) VALUES 
('Apple', 50),
('Orange', 30),
('Banana', 20);



ALTER TABLE goods ADD COLUMN price INTEGER DEFAULT 0;



SELECT * FROM goods;



ALTER TABLE goods MODIFY COLUMN price NUMERIC(8, 2);



ALTER TABLE goods MODIFY COLUMN price INTEGER;



ALTER TABLE goods RENAME COLUMN price TO item_price;


ALTER TABLE goods DROP COLUMN item_price;

