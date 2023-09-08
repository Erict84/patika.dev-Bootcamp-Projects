# Ödev 9

Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.

1. **city** tablosu ile **country** tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
2. **customer** tablosu ile **payment** tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
3. **customer** tablosu ile **rental** tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

# YANITLAR

1.

```sql
SELECT city.city, country.country
FROM country
INNER JOIN city
ON country.country_id = city.country_id;
```

2.

```sql
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM payment
INNER JOIN customer
ON payment.customer_id = customer.customer_id;
```

3.

```sql
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM rental
INNER JOIN customer
ON rental.customer_id = customer.customer_id;
```