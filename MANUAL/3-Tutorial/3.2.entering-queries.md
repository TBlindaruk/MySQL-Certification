#### 3.2 Entering Queries

https://dev.mysql.com/doc/refman/5.6/en/entering-queries.html

```SQL
SELECT VERSION(), CURRENT_DATE;
```

| `VERSION()` | `CURRENT_DATE` |
| ----------- | -------------  |
| 5.7.20-0ubuntu0.16.04.1 |	2017-12-25 |

--------------------------

<strong> Keywords may be entered in any lettercase. The following queries are equivalent:</strong>

```SQL
mysql> SELECT VERSION(), CURRENT_DATE;
mysql> select version(), current_date;
mysql> SeLeCt vErSiOn(), current_DATE;
```

-------------------------

<strong>Here is another query. It demonstrates that you can use mysql as a simple calculator:</strong>
```SQL
mysql> SELECT SIN(PI()/4), (4+1)*5;
```

| SIN(PI()/4)      | (4+1)*5 |
|------------------|---------|
| 0.70710678118655 |      25 |

-----------------------------

<strong>The queries shown thus far have been relatively short, single-line statements. You can even enter multiple statements on a single line. Just end each one with a semicolon:</strong>

```SQL
mysql> SELECT VERSION(); SELECT NOW();
```

| VERSION()    |
| ------------ |
| 5.6.1-m4-log |

| NOW()               |
| ------------------- |
| 2010-08-06 12:17:13 |

-----------------
