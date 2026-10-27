1. Show customers who come from brazil or italy.

SELECT * FROM Customers where country='Brazil' or country='Italy';


2. Display Customers who have the word ‘son’ in their CustomerName. 
SELECT * FROM Customers where customername like '%son%'

3. Display orders made in the month of October 1996, display in asc order.
SELECT * FROM orders WHERE orderdate>='1996-10-01' and orderdate<'1996-11-01' ORDER BY orderdate ASC;

select * from orders where orderdate like '%1996-10%' ORDER BY orderdate ASC;

select * from orders where orderdate between '1996-10-01' and '1996-10-31' ORDER BY orderdate ASC;

4. Find the total orders shipped by each of the 3 shippers.

5. Display products whose price is above 25 from the highest price.

select * from products where price>25 order by price desc;


6. Find the top supplier of the business 
