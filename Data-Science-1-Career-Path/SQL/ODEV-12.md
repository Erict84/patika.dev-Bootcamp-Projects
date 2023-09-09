# Ödev 12

Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.

1. **film** tablosunda film uzunluğu **length** sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
2. **film** tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
3. **film** tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
4. **payment** tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

# YANITLAR

1. 

```sql
SELECT COUNT(*) FROM film
WHERE length > 
(SELECT AVG(length) FROM film);
```

1. 

```sql
SELECT COUNT(*) FROM film
WHERE rental_rate =
(SELECT MAX(rental_rate) FROM FILM);
```

1. 

```sql
SELECT title FROM film
WHERE rental_rate =
(SELECT MIN(rental_rate) FROM film)
AND replacement_cost =
(SELECT MIN(replacement_cost) FROM film);
```

1. 

```sql
SELECT payment.customer_id, COUNT(payment.customer_id), customer.first_name, customer.last_name FROM payment
LEFT JOIN customer
ON payment.customer_id = customer.customer_id
GROUP BY DISTINCT(payment.customer_id), customer.first_name, customer.last_name
ORDER BY COUNT(payment.customer_id) DESC;
```