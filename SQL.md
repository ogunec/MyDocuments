# SQL SELECT
**SELECT** ifadesi, bir veritabanından veri seçmek için kullanılır.  

`SELECT * FROM Customers;` => Customers isimli tabloya ait bütün sütunları getiririz.  
`SELECT CustomerName, City FROM Customers` => Customers isimli tabloda yer alan CustomerName ve City sütunlarını getirir.

## SQL SELECT DISTINCT
SELECT DISTINCT ifadesi, yalnızca farklı değerleri döndürmek için kullanılır.  
`SELECT DISTINCT Country FROM Customers;` => Customers isimli tabloda yer alan ülke sütununda yinelenen ifadeleri çıkartır.

# SQL WHERE
WHERE ifadesi, yalnızca belirli bir koşulu sağlayan kayıtları elde etmek için kayıtları filtreleme görevi görür.  
```
SELECT * FROM Customers
WHERE Country='Mexico';
```
## WHERE Operatörleri
| Operatör   | Tanımı       |
|------------|--------------|
| =          | Eşittir      |
| >          | Büyüktür     |
| <          | Küçüktür     |
| >=         | Büyük eşittir|
| <=         | Küçük eşittir|
| !=         | Eşit değil   |
| BETWEEN    | Arasında     |
| LIKE       | Desen ara    |
| IN         | Bir sütun için birden fazla olası değer belirtme |
