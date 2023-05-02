1. film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
2. film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
3. customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.



1 Cevap

```
select title from film where title like '%n'order by title limit 5;
```

2 Cevap

```
select title from film where title like '%n'order by title offset 5 limit 5;
```

3 Cevap

```
select last_name from customer where store_id in (1) order by last_name desc limit 4;
```


