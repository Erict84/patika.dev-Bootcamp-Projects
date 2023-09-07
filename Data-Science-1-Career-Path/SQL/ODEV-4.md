# ODEV 4

> Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.
> 
1. **film** tablosunda bulunan **replacement_cost** sütununda bulunan birbirinden farklı değerleri sıralayınız.
2. **film** tablosunda bulunan **replacement_cost** sütununda birbirinden farklı kaç tane veri vardır?
3. **film** tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
4. **country** tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
5. **city** tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

# YANITLAR

1. **film** tablosunda bulunan **replacement_cost** sütununda bulunan birbirinden farklı değerleri sıralayınız.

```sql
SELECT DISTINCT replacement_cost FROM film;
```

1. **film** tablosunda bulunan **replacement_cost** sütununda birbirinden farklı kaç tane veri vardır?

```sql
SELECT COUNT(DISTINCT replacement_cost) FROM film;
```

1. **film** tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

```sql
SELECT COUNT(title) from film WHERE title like 'T%' AND rating = 'G';
```

1. **country** tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

```sql
SELECT COUNT(country) FROM country WHERE country LIKE '_____';
```

1. **city** tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

```sql
SELECT COUNT(city) FROM city WHERE city ILIKE '%r';
```