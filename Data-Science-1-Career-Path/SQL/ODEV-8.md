# Ödev 8

1. **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
2. Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

1. 

```sql
CREATE TABLE employee (
id INTEGER,
name VARCHAR(50),
birthday DATE,
email VARCHAR(100)
);
```

2.

```sql
insert into employee (id, name, birthday, email) values (1, 'Tish Cough', '1932-02-07', 'tcough0@shutterfly.com');
insert into employee (id, name, birthday, email) values (2, 'Ellis Churchley', '1941-05-27', 'echurchley1@wsj.com');
insert into employee (id, name, birthday, email) values (3, 'Riki Dillingstone', '1928-07-12', 'rdillingstone2@reference.com');
insert into employee (id, name, birthday, email) values (4, 'Stefania Magson', '1984-03-26', 'smagson3@privacy.gov.au');
insert into employee (id, name, birthday, email) values (5, 'Georgina Biaggiotti', '1951-09-29', 'gbiaggiotti4@sfgate.com');
insert into employee (id, name, birthday, email) values (6, 'Truman Blackshaw', '1978-06-30', 'tblackshaw5@nationalgeographic.com');
insert into employee (id, name, birthday, email) values (7, 'Iorgos Sturgis', '1962-10-07', 'isturgis6@typepad.com');
insert into employee (id, name, birthday, email) values (8, 'Yasmin MacTeggart', '1942-01-03', 'ymacteggart7@blogtalkradio.com');
insert into employee (id, name, birthday, email) values (9, 'Agnola Toping', '1923-12-27', 'atoping8@theglobeandmail.com');
insert into employee (id, name, birthday, email) values (10, 'Philipa Goody', '1934-03-29', 'pgoody9@posterous.com');
insert into employee (id, name, birthday, email) values (11, 'Georas Cundey', '1915-12-11', 'gcundeya@ning.com');
insert into employee (id, name, birthday, email) values (12, 'Wilma Illwell', '1975-09-02', 'willwellb@eepurl.com');
insert into employee (id, name, birthday, email) values (13, 'Tammie Hudson', '1962-09-02', 'thudsonc@google.com');
insert into employee (id, name, birthday, email) values (14, 'Ezequiel Segebrecht', '1987-08-08', 'esegebrechtd@geocities.com');
insert into employee (id, name, birthday, email) values (15, 'Darwin Cotter', '1954-03-23', 'dcottere@sakura.ne.jp');
insert into employee (id, name, birthday, email) values (16, 'Del Menlow', '1933-10-31', 'dmenlowf@behance.net');
insert into employee (id, name, birthday, email) values (17, 'Fritz Sirrell', '1927-02-04', 'fsirrellg@netvibes.com');
insert into employee (id, name, birthday, email) values (18, 'Paola Cranstone', '1960-05-21', 'pcranstoneh@icq.com');
insert into employee (id, name, birthday, email) values (19, 'Nevile Uden', '1904-01-13', 'nudeni@census.gov');
insert into employee (id, name, birthday, email) values (20, 'Crista Oganesian', '1935-10-12', 'coganesianj@constantcontact.com');
insert into employee (id, name, birthday, email) values (21, 'Maegan Symons', '1947-11-13', 'msymonsk@mediafire.com');
insert into employee (id, name, birthday, email) values (22, 'Cale Duny', '1985-07-11', 'cdunyl@livejournal.com');
insert into employee (id, name, birthday, email) values (23, 'Justus Crichmere', '1943-05-16', 'jcrichmerem@mapy.cz');
insert into employee (id, name, birthday, email) values (24, 'Esme Edgeon', '1951-03-28', 'eedgeonn@state.tx.us');
insert into employee (id, name, birthday, email) values (25, 'Svend Piatek', '1908-08-14', 'spiateko@cdc.gov');
insert into employee (id, name, birthday, email) values (26, 'Kincaid Bowie', '1918-06-21', 'kbowiep@who.int');
insert into employee (id, name, birthday, email) values (27, 'Edithe Irdale', '1912-03-27', 'eirdaleq@apache.org');
insert into employee (id, name, birthday, email) values (28, 'Staford Struys', '1916-09-21', 'sstruysr@infoseek.co.jp');
insert into employee (id, name, birthday, email) values (29, 'Kerrin Outerbridge', '1919-11-14', 'kouterbridges@dmoz.org');
insert into employee (id, name, birthday, email) values (30, 'Blane Burnhard', '1923-11-08', 'bburnhardt@indiegogo.com');
insert into employee (id, name, birthday, email) values (31, 'Vitoria Gumey', '1917-07-19', 'vgumeyu@bloomberg.com');
insert into employee (id, name, birthday, email) values (32, 'Laetitia Marsh', '1953-04-21', 'lmarshv@odnoklassniki.ru');
insert into employee (id, name, birthday, email) values (33, 'Byram Pedri', '1965-05-12', 'bpedriw@who.int');
insert into employee (id, name, birthday, email) values (34, 'Burg Curnock', '1979-11-29', 'bcurnockx@squarespace.com');
insert into employee (id, name, birthday, email) values (35, 'Cesare Fernanando', '1961-03-01', 'cfernanandoy@yandex.ru');
insert into employee (id, name, birthday, email) values (36, 'Michaelina Georgi', '1931-01-08', 'mgeorgiz@accuweather.com');
insert into employee (id, name, birthday, email) values (37, 'Frannie Taffee', '1918-06-01', 'ftaffee10@cbsnews.com');
insert into employee (id, name, birthday, email) values (38, 'Virginia Astill', '1933-04-04', 'vastill11@jugem.jp');
insert into employee (id, name, birthday, email) values (39, 'Kassia Allardyce', '1958-01-22', 'kallardyce12@csmonitor.com');
insert into employee (id, name, birthday, email) values (40, 'Deerdre Domotor', '1933-11-13', 'ddomotor13@ucla.edu');
insert into employee (id, name, birthday, email) values (41, 'Reagan Borrington', '1981-01-11', 'rborrington14@ocn.ne.jp');
insert into employee (id, name, birthday, email) values (42, 'La verne Ingleton', '1927-03-03', 'lverne15@facebook.com');
insert into employee (id, name, birthday, email) values (43, 'Neila Gaffey', '1934-08-23', 'ngaffey16@slashdot.org');
insert into employee (id, name, birthday, email) values (44, 'Maury Soan', '1912-06-24', 'msoan17@bloglovin.com');
insert into employee (id, name, birthday, email) values (45, 'Rochelle Cosley', '1921-01-11', 'rcosley18@google.co.jp');
insert into employee (id, name, birthday, email) values (46, 'Pandora Van T''Hoog', '1911-04-06', 'pvan19@whitehouse.gov');
insert into employee (id, name, birthday, email) values (47, 'Chelsey Cappleman', '1948-10-25', 'ccappleman1a@cargocollective.com');
insert into employee (id, name, birthday, email) values (48, 'Errol Stormonth', '1973-09-05', 'estormonth1b@phoca.cz');
insert into employee (id, name, birthday, email) values (49, 'Faustine Crehan', '1922-09-13', 'fcrehan1c@friendfeed.com');
insert into employee (id, name, birthday, email) values (50, 'Jasen Beaglehole', '1970-11-18', 'jbeaglehole1d@wp.com');
```

3.

```sql
UPDATE employee
SET birthday = NULL
WHERE email LIKE 'b%'
RETURNING *;
```

```sql
UPDATE employee
SET birthday = '1954-12-31'
WHERE name LIKE 'Blane%'
RETURNING *;
```

```sql
UPDATE employee
SET name = '30lular'
WHERE birthday > '1930-01-01' AND birthday < '1940-01-01'
RETURNING *;
```

```sql
UPDATE employee
SET name = 'Ruslar'
WHERE email LIKE '%.ru'
RETURNING *;
```

```sql
UPDATE employee
SET name = 'Ilk 10'
WHERE id < 11
RETURNING *;
```

4.

```sql
DELETE FROM employee
WHERE id = 10
RETURNING *;
```

```sql
DELETE FROM employee
WHERE name = 'Ruslar'
RETURNING *;
```

```sql
DELETE FROM employee 
WHERE birthday > '1939-12-31' AND birthday < '1950-01-01'
RETURNING *;
```

```sql
DELETE FROM employee
WHERE email LIKE '%jp'
RETURNING *;
```

```sql
DELETE FROM employee
WHERE id BETWEEN 20 AND 30
RETURNING *;
```