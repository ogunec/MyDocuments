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
