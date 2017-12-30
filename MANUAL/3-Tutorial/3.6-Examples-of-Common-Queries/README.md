### 3.6 Examples of Common Queries

<strong>
You can create and populate the example table with these statements:
</strong>

```SQL
CREATE TABLE shop (
    article INT(4) UNSIGNED ZEROFILL DEFAULT '0000' NOT NULL,
    dealer  CHAR(20)                 DEFAULT ''     NOT NULL,
    price   DOUBLE(16,2)             DEFAULT '0.00' NOT NULL,
    PRIMARY KEY(article, dealer));
INSERT INTO shop VALUES
    (1,'A',3.45),(1,'B',3.99),(2,'A',10.99),(3,'B',1.45),
    (3,'C',1.69),(3,'D',1.25),(4,'D',19.95);
```

<p>After issuing the statements, the table should have the following contents:</p>

```SQL
SELECT * FROM shop;
```

| article | dealer | price |
|---------|--------|-------|
|    1 | A      |  3.45 |
|    1 | B      |  3.99 |
|    2 | A      | 10.99 |
|    3 | B      |  1.45 |
|    3 | C      |  1.69 |
|    3 | D      |  1.25 |
|    4 | D      | 19.95 |