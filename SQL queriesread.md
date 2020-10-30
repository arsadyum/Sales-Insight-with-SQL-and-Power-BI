# Data Analysis Using SQL
## Show all customer records

SELECT * FROM customers;

## Show total number of customers

SELECT count(*) FROM customers;

## Show transactions for  market (market code for NewYork is MarK097

SELECT * FROM transactions where market_code='Mark097';

## Show distrinct product codes that were sold in Mumbai

SELECT distinct product_code FROM transactions where market_code='Mark002';

## Show transactions where currency is US dollars

SELECT * from transactions where currency="USD"

## Show transactions in 2020 join by date table

SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

## Show total revenue in year 2020,

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";

## Show total revenue in year 2020, January Month,

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");

## Show total revenue in year 2020 in Kanpur

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark005";

# Check for duplicates with below queries 
SELECT DISTINCT(transactions.currency) from transactions;

SELECT count(*) from transactions where transactions.currency = 'INR\r' ;

SELECT count(*) from transactions where transactions.currency = 'INR';

SELECT count(*) from transactions where transactions.currency = 'USD';
SELECT count(*) from transactions where transactions.currency = 'USD\r';

select * from transactions where transactions.currency = 'USD' or transactions.currency = 'USD\r';

select * from transactions where transactions.currency = 'INR' or transactions.currency = 'INR\r'; 
