1. film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
2. film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
3. film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
4. country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
5. city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?



1 Cevap

```sql
select distinct replacement_cost from film;
```

2 Cevap

```sql
select count (replacement_cost) from film;
```

3 Cevap

```sql
select count(*) from film where title like ('T%') and rating = 'G';
```

4 Cevap

```sql
select count(city) from city where city like ('R%r');
```

5 Cevap

```sql
select count(country) from country where country like ('_____');
```







