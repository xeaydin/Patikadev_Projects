* Sort the data in the title and description columns in the film table.


```sql
SELECT title, description
FROM film;
```


* Sort the data in all columns in the film table with the film length greater than 60 AND less than 75.


```sql
SELECT *
FROM film
WHERE length > 60 AND length < 70;
```



* Sort the data in all columns in the film table with rental_rate 0.99 AND replacement_cost 12.99 OR 28.99.


```sql
SELECT *
FROM film
WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);
```


 
* What is the value in the last_name column of the customer whose value is 'Mary' in the first_name column of the customer table?


```sql
SELECT last_name
FROM customer
WHERE first_name='Mary';
```



* Sort the data in the film table whose length is NOT greater than 50, but whose rental_rate is NOT 2.99 or 4.99.

```sql
SELECT *
FROM film
WHERE length <= 50 AND NOT(rental_rate=2.99 OR rental_rate=4.99);
```
