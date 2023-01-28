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
| BETWEEN    | Belirli bir aralık arasında |
| LIKE       | Belirli bir paterni arama |
| IN         | Bir sütun için birden fazla olası değer belirtme |

# SQL AND, OR ve NOT
WHERE ifadesi AND, OR ve NOT işleçleriyle birleştirilebilir.  
* AND operatörü, AND ile ayrılan tüm koşullar DOĞRU ise bir kayıt görüntüler.
* OR ile ayrılan koşullardan herhangi biri DOĞRU ise OR operatörü bir kayıt görüntüler.
* NOT operatörü, koşul(lar) DOĞRU DEĞİL ise bir kayıt görüntüler.  
```
SELECT * FROM Customers
WHERE Country='Germany' AND City='Berlin';

SELECT * FROM Customers
WHERE City='Berlin' OR City='München';

SELECT * FROM Customers
WHERE NOT Country='Germany';
```
## AND, OR ve NOT'u Birlikte Kullanma
Aşağıdaki SQL ifadesi, "Customers" tablosundan ülkesi Almanya şehri Berlin veya Münih olanları seçer.  
```
SELECT * FROM Customers
WHERE Country='Germany' AND (City='Berlin' OR City='München');
```
Aşağıdaki SQL ifadesi, Customers tablosundan ülkesi Almanya ve USA olmayan tüm alanları seçer.  
```
SELECT * FROM Customers
WHERE NOT Country='Germany' AND NOT Country='USA';
```
# SQL ORDER BY
* ORDER BY anahtar sözcüğü, sonuç kümesini artan veya azalan düzende sıralamak için kullanılır.
* ORDER BY anahtar sözcüğü, kayıtları varsayılan olarak artan düzende sıralar. Kayıtları azalan düzende sıralamak için DESC anahtar sözcüğünü kullanın.
```
Aşağıda yer alan ifade Customers tablosunda yer alan müşterileri ülkelerine göre artan düzende sıralar.

SELECT * FROM Customers
ORDER BY Country;

Aşağıdaki SQL ifadesi, "Customers" tablosundan "Country" sütununa göre DESCENDING olarak sıralanan tüm müşterileri getirir.

SELECT * FROM Customers
ORDER BY Country DESC;
```
## ORDER BY Farklı Sütunlarda Sıralama
Aşağıdaki SQL deyimi, "Country" ve "CustomerName" sütununa göre sıralanmış "Customers" tablosundan tüm müşterilerini seçer. Bu, "Country" sütununa göre sıralandığı anlamına gelir, ancak bazı satırlar aynı olma durumunda, bunları "CustomerName" sütununa göre sıralayacaktır.
```
SELECT * FROM Customers
ORDER BY Country, CustomerName;
```
# SQL INSERT INTO
INSERT INTO ifadesi, bir tabloya yeni kayıtlar eklemek için kullanılır.
INSERT INTO deyimini iki şekilde yazmak mümkündür;
* Hem sütun adlarını hem de eklenecek değerleri belirtin.
```
INSERT INTO Customers (CustomerName, ContactName, Address, City, PostalCode, Country)
VALUES ('Cardinal', 'Tom B. Erichsen', 'Skagen 21', 'Stavanger', '4006', 'Norway');
```
* Tablonun tüm sütunları için değer ekliyorsanız, SQL sorgusunda sütun adlarını belirtmeniz gerekmez. Ancak, değerlerin sırasının tablodaki sütunlarla aynı sırada olduğundan emin olun.
```
INSERT INTO Customers
VALUES (92,'Cardinal', 'Tom B. Erichsen', 'Skagen 21', 'Stavanger', '4006', 'Norway');
```
# SQL NULL
* NULL değeri olan bir alan, değeri olmayan bir alandır.
* NULL değeri, sıfır değerinden veya boşluk içeren bir alandan farklıdır. NULL değerine sahip bir alan, kayıt oluşturma sırasında boş bırakılan bir alandır!
* NULL olup olmadığını test etmek için IS NULL ve IS NOT NULL operatörlerini kullanacağız.
```
SELECT CustomerName, ContactName, Address
FROM Customers
WHERE Address IS NULL;

SELECT CustomerName, ContactName, Address
FROM Customers
WHERE Address IS NOT NULL;
```
# SQL UPDATE
* UPDATE deyimi, bir tablodaki mevcut kayıtları değiştirmek için kullanılır.
* Update yaparken WHERE ifadesi hangi kayıtların güncellenmesi gerektiğini belirtir. WHERE ifadesi olmazsa, tablodaki tüm kayıtlar güncellenir!
```
UPDATE Customers
SET ContactName = 'Alfred Schmidt', City= 'Frankfurt'
WHERE CustomerID = 1;
```
# SQL DELETE
* DELETE ifadesi, bir tablodaki mevcut kayıtları silmek için kullanılır.
* Delete yaparken WHERE ifadesi hangi kayıtların silinmesi gerektiğini belirtir. WHERE ifadesi olmazsa, tablodaki tüm kayıtlar silinir!  
```
DELETE FROM Customers
WHERE CustomerName='Alfreds Futterkiste';
```
# SQL SELECT TOP
* SELECT TOP ifadesi, döndürülecek kayıt sayısını belirtmek için kullanılır.
* SELECT TOP ifadesi PERCENT ifadesi ile kullanılarak elde edilmek istenen veri sayısı yüzdesel olarakta belirtilebilir.
* SELECT TOP ifadesi WHERE ifadesi ile birlikte kullanılarak gerekli şartı sağlayan belli sayıdaki veri elde edilebilir.
```
SELECT TOP 3 * FROM Customers;

SQL TOP PERCENT
SELECT TOP 50 PERCENT * FROM Customers;

WHERE CLAUSE
SELECT TOP 3 * FROM Customers
WHERE Country='Germany';
```
# SQL MIN() ve MAX() Fonsiyonları
* MIN() fonksiyonu, seçilen sütunun en küçük değerini döndürür.
* MAX() fonlsiyonu, seçilen sütunun en büyük değerini döndürür.
```
SELECT MIN(Price) AS SmallestPrice
FROM Products;

SELECT MAX(Price) AS LargestPrice
FROM Products;
```
# SQL COUNT(), AVG() ve SUM() Fonksiyonları
* COUNT() fonksiyonu, belirtilen bir ölçütle eşleşen satır sayısını döndürür.
* SUM() fonksiyonu, bir sayısal sütunun toplamını döndürür.
* AVG() fonksiyonu, sayısal bir sütunun ortalama değerini döndürür.
```
SELECT COUNT(ProductID)
FROM Products;

SELECT AVG(Price)
FROM Products;

SELECT SUM(Quantity)
FROM OrderDetails;
```
# SQL LIKE
* LIKE operatörü, bir sütunda belirli bir kalıbı aramak için bir WHERE ifadesiyle kullanılır.
* LIKE operatörüyle birlikte sıklıkla kullanılan iki sembol vardır. Bunlar "%" ve "_" sembolleri.  

## SQL Wildcards

| LIKE Operatörü | Tanımı         |
|----------------|----------------|
| WHERE CustomerName LIKE 'a%' | "a" ile başlayan tüm değerleri bulur |
| WHERE CustomerName LIKE '%a' | "a" ile biten tüm değerleri bulur|
| WHERE CustomerName LIKE '%or%' | Herhangi bir konumda "or" içeren tüm değerleri bulur |
| WHERE CustomerName LIKE '_r%' | İkinci harfi "r" olan tüm değerleri bulur |
| WHERE CustomerName LIKE 'a_% | "a" ile başlayan ve en az 2 karakter uzunluğunda olan tüm değerleri bulur |
| WHERE CustomerName LIKE 'a__%' | "a" ile başlayan ve en az 3 karakter uzunluğunda olan tüm değerleri bulur |
| WHERE ContactName LIKE 'a%o' | "a" ile başlayan ve "o" ile biten tüm değerleri bulur |
| WHERE ContactName LIKE '[bsp]%' | "b", "s" veya "p" ile başlayan tüm ifadeleri bulur |
| WHERE ContactName LIKE '[a-c]%' | "a", "b" veya "c" ile başlayan tüm ifadeleri bulur. |
| WHERE ContactName LIKE '[!bsp]%' | "b", "s" veya "p" ile başlamayan tüm ifadeleri bulur |
```
SELECT * FROM Customers
WHERE CustomerName LIKE 'a%';

SELECT * FROM Customers
WHERE CustomerName LIKE '%a';

SELECT * FROM Customers
WHERE CustomerName LIKE '%or%';
```
# SQL IN
* IN operatörü, bir WHERE ifadesinde birden çok değer belirtmenize izin verir.
* IN operatörü, birden çok OR koşulu için bir kısayoldur.
```
SELECT * FROM Customers
WHERE Country IN ('Germany', 'France', 'UK');

SELECT * FROM Customers
WHERE Country NOT IN ('Germany', 'France', 'UK');

SELECT * FROM Customers
WHERE Country IN (SELECT Country FROM Suppliers);
```
# SQL BETWEEN
* BETWEEN operatörü, belirli bir aralıktaki değerleri seçer. Değerler sayı, metin veya tarih olabilir.
* BETWEEN operatörü kapsayıcıdır: başlangıç ​​ve bitiş değerleri dahildir.
```
SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20;

SELECT * FROM Products
WHERE Price NOT BETWEEN 10 AND 20;

SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20
AND CategoryID NOT IN (1,2,3);
```
# SQL Aliases
* SQL takma adları, bir tabloya veya tablodaki bir sütuna geçici bir ad vermek için kullanılır.
* Takma ad yalnızca bu sorgunun süresi boyunca mevcuttur.
* AS anahtar sözcüğü ile bir takma ad oluşturulur.
```
SELECT CustomerID AS ID, CustomerName AS Customer
FROM Customers;

SELECT CustomerName, CONCAT(Address,', ',PostalCode,', ',City,', ',Country) AS Address
FROM Customers;

SELECT o.OrderID, o.OrderDate, c.CustomerName
FROM Customers AS c, Orders AS o
WHERE c.CustomerName='Around the Horn' AND c.CustomerID=o.CustomerID;
```
