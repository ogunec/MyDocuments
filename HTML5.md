# HTML Başlıkları
`<h1>, <h2>, <h3>, <h4>, <h5>, <h6>` tagları ile başlıklar atılır. `<h1>` en büyük başlık boyutu `<h6>` ise en küçük başlık boyutunu işaret eder.

`<h1>This is heading 1</h1>`  
`<h2>This is heading 2</h2>`  
`<h3>This is heading 3</h3>`  
`<h4>This is heading 4</h4>`  
`<h5>This is heading 5</h5>`  
`<h6>This is heading 6</h6>`  

# HTML Paragrafları
HTML paragrafları `<p>` etiketi ile tanımlanır  

`<p>This is a paragraph.</p>`  
`<p>This is another paragraph.</p>`  

`<pre>` etiketi önceden biçimlendirilmiş metin tanımlar. Metnin satır sonları ve boşlukları korunur.  


# HTML Link
* HTML bağlantıları `<a>` etiketi ile tanımlanır.  

`<a href="https://www.google.com.com">Google</a>`  

* Bağlantının hedefi, `href` niteliği ile belirtilir.    
* Oluşturulan linkin nerede açılacağını `target` niteliği belirtir. `target` özniteliği aşağıdaki değerlerden birine sahip olabilir.  
`_self` - Varsayılan. Belgeyi tıklandığı pencerede/sekmede açar.  
`_blank` - Belgeyi yeni bir pencerede veya sekmede açar.  

`<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>`  
## Bir Görüntüyü Bağlantı Olarak Kullan
Bir görseli bağlantı olarak kullanmak için <img> etiketini <a> etiketinin içine koymanız yeterlidir.  
```
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```
## Bir E-posta Adresine Bağlantı
Kullanıcının e-posta programını açan bir bağlantı oluşturmak için `href` özniteliği içinde `mailto:` öğesini kullanın.  
`<a href="mailto:someone@example.com">Send email</a>`  
  
## Butona Bağlantı
Bir HTML düğmesini bağlantı olarak kullanmak için bazı JavaScript kodları eklemeniz gerekir.  
`<button onclick="document.location='default.asp'">HTML Tutorial</button>`  
## Link Başlığı
`title` niteliği, bir öğe hakkında ek bilgi belirtir. Bilgi, çoğunlukla fare öğenin üzerine geldiğinde bir araç ipucu metni olarak gösterilir.
`<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>`  

  
# HTML Resimleri
HTML görselleri `<img>` etiketi ile tanımlanır.  
Kaynak dosya `src`, alternatif metin `alt`, genişlik `width` ve yükseklik `height`, nitelikleri ile sağlanır.  

`<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">`  

# Boş HTML Öğeleri
* İçeriği olmayan HTML öğelerine boş öğeler denir. `<br>` etiketi bir satır sonu tanımlar ve kapanış etiketi olmayan boş bir öğedir.  
`<p>This is a <br> paragraph with a line break.</p>`  

* `<hr>` etiketi HTML5 ile görsel açıdan yatay bir çizgi çekerek belgede bir konu sonu tanımlar.  

# HTML Nitelikleri
Tüm HTML öğelerinin nitelikleri olabilir  
Nitelikler, öğeler hakkında ek bilgi sağlar  
Nitelikler her zaman başlangıç ​​etiketinde belirtilir  
Nitelikler genellikle aşağıdaki gibi ad/değer çiftleri halinde gelir: name="value"    

## Bazı HTML Nitelikleri
* `<a>` etiketi bir link tanımlar. `href` niteliği ise bağlantının gittiği sayfanın URL'sini belirtir.  
`<a href="https://www.w3schools.com">Visit W3Schools</a>`  

* `<img>` etiketi, bir resim dosyasını HTML sayfasına gömmek için kullanılır. `src` niteliği ise resim dosyasının yolunu belirtir.  
`<img src="img_girl.jpg">`  

* `alt` niteliği, resim herhangi bir nedenle gösterilemiyorsa, resim için alternatif bir metin belirtir.  
`<img src="img_girl.jpg" alt="Girl with a jacket">`  

* `<img>` etiketi, görüntünün genişliğini ve yüksekliğini (piksel cinsinden) belirten `width` ve `height` niteliklerini de içermelidir.  
`<img src="img_girl.jpg" width="500" height="600">`  

* `style` niteliği, bir öğeye renk, yazı tipi, boyut ve daha fazlası gibi stiller eklemek için kullanılır.  
`<p style="color:red;">This is a red paragraph.</p>`

* Web sayfasının dilini bildirmek için her zaman `<html>` etiketinin içine `lang` niteliğini eklemelisiniz. Bu, arama motorlarına ve tarayıcılara yardımcı olmak içindir.  
`<html lang="en">`  

* `title` niteliği, bir öğe hakkında bilgileri tanımlar. `title` özniteliğinin değeri, öğenin üzerine fareyi getirdiğinizde görüntülenecektir.  
`<p title="I'm a tooltip">This is a paragraph.</p>`  

# HTML Style Niteliği
HTML `atyle` niteliği, bir öğeye renk, yazı tipi, boyut ve daha fazlası gibi stiller eklemek için kullanılır.  
`<tagname style="property:value;">` Burada property bir CSS özelliği ve value bir CSS değeridir.  

## Bazı Style Özellikleri
* Backgroun Color: CSS `background-color` özelliği, bir HTML öğesi için arka plan rengini tanımlar.  
`<h1 style="background-color:powderblue;">This is a heading</h1>`  

* Text Color: CSS `color` özelliği, bir HTML öğesi için metin rengini tanımlar.  
`<p style="color:red;">This is a paragraph.</p>`  

* Fonts: CSS `font-family` özelliği, bir HTML öğesi için kullanılacak yazı tipini tanımlar.  
`<h1 style="font-family:verdana;">This is a heading</h1>`  

* Text Size: CSS `font-size` özelliği, bir HTML öğesinin metin boyutunu tanımlar.  
`<p style="font-size:160%;">This is a paragraph.</p>`  

* Text Alignment: CSS `text-align` özelliği, bir HTML öğesi için yatay metin hizalamasını tanımlar.  
`<p style="text-align:center;">Centered paragraph.</p>`  

# HTML Metin Biçimlendirme
* `<b>` öğesi, kalın metni herhangi bir ekstra önem olmaksızın tanımlar.  
* `<strong>` öğesi, metni büyük önemle tanımlar. İçerideki içerik genellikle kalın olarak görüntülenir.  
* `<i>` öğesi, metnin bir bölümünü alternatif bir ses veya ruh halinde tanımlar. İçerideki içerik tipik olarak italik olarak görüntülenir.  
* `<em>` öğesi, vurgulanan metni tanımlar. İçerideki içerik tipik olarak italik olarak görüntülenir.  
* `<mark>` öğesi, işaretlenmesi veya vurgulanması gereken metni tanımlar.  
* `<small>` öğesi daha küçük metni tanımlar.  
* `<del>` öğesi, bir belgeden silinmiş olan metni tanımlar. Tarayıcılar genellikle silinen metin boyunca bir satır çizer.  
* `<ins>` öğesi, bir belgeye eklenmiş bir metni tanımlar. Tarayıcılar genellikle eklenen metnin altını çizer.  
* `<sub>` öğesi, alt simge metnini tanımlar. Alt simge metni, normal satırın yarım karakter altında görünür ve bazen daha küçük bir yazı tipiyle işlenir. Alt simge metni, H2O gibi kimyasal formüller için kullanılabilir.  
* `<sup>` öğesi, üst simge metnini tanımlar. Üst simge metni, normal satırın yarım karakter üzerinde görünür ve bazen daha küçük bir yazı tipiyle işlenir.  

# HTML Alıntılar
* `<blockquote>` öğesi, başka bir kaynaktan alıntılanan bir bölümü tanımlar. Tarayıcılar genellikle `<blockquote>` öğelerini girintiler.
* `<q>` etiketi kısa bir alıntıyı tanımlar. Tarayıcılar normalde alıntının etrafına tırnak işaretleri ekler.  
* `<abbr>` etiketi, "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM" gibi kısaltmaları tanımlar.  
İpucu: Fareyi öğenin üzerine getirdiğinizde kısaltmanın açıklamasını göstermek için `title` özniteliğini kullanın.  
`<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>`  
* `<address>` etiketi, bir belgenin veya makalenin yazarı/sahibi için iletişim bilgilerini tanımlar.  
* `<cite>` etiketi, yaratıcı bir çalışmanın başlığını tanımlar (ör. bir kitap, bir şiir, bir şarkı, bir film, bir tablo, bir heykel vb.).  
* `<bdo>` etiketi, geçerli metin yönünü geçersiz kılmak için kullanılır.  
`<bdo dir="rtl">This text will be written from right to left</bdo>`

# HTML Yorum Satırı
HTML yorumları tarayıcıda görüntülenmez ancak HTML kaynak kodunuzu belgelemenize yardımcı olabilir.  
`<!-- Write your comments here -->`  

HTML kodumuza yorum satırı eklemek ve geçici süreyle görünmesini istemediğimiz içerikleri saklamak amacıyla kullanabiliriz.  
`<!-- <p>This is another paragraph </p> -->`  
`<p>This <!-- great text --> is a paragraph.</p>`  

# HTML Renkler
HTML renkleri, önceden tanımlanmış renk adlarıyla veya RGB, HEX, HSL, RGBA veya HSLA değerleriyle belirtilir.  
* Text Color: Metnin rengini ayarlayabilirsiniz.  
`<h1 style="color:Tomato;">Hello World</h1>`  
* Border Color: Kenarlıkların rengini ayarlayabilirsiniz.  
`<h1 style="border:2px solid Tomato;">Hello World</h1>`  
* Background Color: Arkaplanın rengini ayarlayabilirsiniz.  
`<h1 style="background-color:Tomato;">Hello World</h1>`  

## Renk Değerleri
HTML'de renkler, RGB değerleri, HEX değerleri, HSL değerleri, RGBA değerleri ve HSLA değerleri kullanılarak da belirtilebilir.  
Aşağıdaki üç `<div>` öğesinin arka plan rengi RGB, HEX ve HSL değerleriyle ayarlanır.  
`<h1 style="background-color:rgb(255, 99, 71);">...</h1>`  
`<h1 style="background-color:#ff6347;">...</h1>`  
`<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>`  
Aşağıdaki iki `<div>` öğesinin arka plan rengi RGBA ve HSLA değerleriyle ayarlanmıştır. 
`<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>`  
`<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>`

### RGB Renk Değerleri
* Bir RGB renk değeri, KIRMIZI, YEŞİL ve MAVİ ışık kaynaklarını temsil eder.  
* Her parametre (kırmızı, yeşil ve mavi), rengin yoğunluğunu 0 ile 255 arasında bir değerle tanımlar.  
* Örneğin, rgb(255, 0, 0) kırmızı olarak görüntülenir çünkü kırmızı en yüksek değerine (255) ve diğer ikisi (yeşil ve mavi) 0'a ayarlanmıştır.  
* Siyahı görüntülemek için tüm renk parametrelerini şu şekilde 0 olarak ayarlayın: rgb(0, 0, 0).  
* Beyazı görüntülemek için tüm renk parametrelerini 255 olarak ayarlayın, örneğin: rgb(255, 255, 255).  
* Grinin tonları genellikle üç parametrenin tümü için eşit değerler kullanılarak tanımlanır, örneğin: rgb(180, 180, 180).  
* rgba(red, green, blue, alpha) renk değerleri, bir rengin opaklığını belirten bir Alfa kanalıyla RGB renk değerlerinin bir uzantısıdır. alpha parametresi 0.0 (tamamen şeffaf) ile 1.0 (hiç şeffaf değil) arasında bir sayıdır.  

### HEX Renk Değerleri
* #rrggbb rr (kırmızı), gg (yeşil) ve bb (mavi), 00 ile ff arasındaki onaltılık değerlerdir (ondalık 0-255 ile aynı).  
* #ff0000 kırmızı olarak görüntülenir çünkü kırmızı en yüksek değerine (ff) ve diğer ikisi (yeşil ve mavi) 00'a ayarlanmıştır.  
* Siyahı görüntülemek için tüm renk parametrelerini 00 olarak ayarlayın, örneğin: #000000.  
* Beyazı görüntülemek için tüm renk parametrelerini ff olarak ayarlayın, örneğin: #ffffff.  
* Grinin tonları genellikle üç parametrenin tümü için eşit değerler kullanılarak tanımlanır. Ör: #f8f8f8.  

### HSL Renk Değerleri
* HTML'de bir renk, şu şekilde ton, doygunluk ve açıklık (HSL) kullanılarak belirtilebilir: hsl(ton, doygunluk, açıklık)   
* Ton, renk tekerleğinde 0 ile 360 ​​arasındaki bir derecedir. 0 kırmızı, 120 yeşil ve 240 mavidir.  
* Doygunluk bir yüzde değeridir. %0, grinin bir tonu ve %100 tam renk anlamına gelir.  
* Açıklık de bir yüzde değeridir. %0 siyah ve %100 beyazdır.  
* Gri tonları genellikle ton ve doygunluğu 0'a ayarlayarak ve daha koyu/açık gölgeler elde etmek için açıklığı %0'dan %100'e ayarlayarak tanımlanır. hsl(0, 0%, 70%)  
* hsla(hue, saturation, lightness, alpha) renk değerleri, bir rengin opaklığını belirten bir Alfa kanalıyla HSL renk değerlerinin bir uzantısıdır.  

# HTML Tablolar
HTML tabloları, web geliştiricilerinin verileri satırlar ve sütunlar halinde düzenlemesine olanak tanır.  
```
<table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```  
<table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>  

# HTML Listeleri
HTML listeleri, web geliştiricilerinin bir dizi ilgili öğeyi listelerde gruplandırmasına olanak tanır.  

## Sıralı Olmayan HTML Listesi
Sırasız bir liste `<ul>` etiketi ile başlar. Her liste öğesi `<li>` etiketi ile başlar.
```
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>  
```
## Sıralı HTML Listesi
Sıralı bir liste `<ol>` etiketi ile başlar. Her liste öğesi `<li>` etiketi ile başlar.  
```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>  
```
### Sıralı Liste Type Özelliği
* type="1" Liste öğeleri sayılarla numaralandırılacaktır (varsayılan)  
* type="A" Liste öğeleri büyük harflerle numaralandırılacaktır.  
* type="a" Liste öğeleri küçük harflerle numaralandırılacaktır.  
* type="I" Liste öğeleri büyük roma rakamlarıyla numaralandırılacaktır.  
* type="i" Liste öğeleri küçük roma rakamlarıyla numaralandırılacaktır.  
```
<ol type="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>  
```
## HTML Açıklama Listesi
Açıklama listesi, her terimin açıklamasını içeren bir terimler listesidir. `<dl>` etiketi açıklama listesini tanımlar, `<dt>` etiketi tanımlanacak terimi belirtir ve `<dd>` etiketi her terimi açıklar.  
```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
# HTML Head Elementi
`<head>` öğesi, meta veriler için bir etikettir ve `<html>` etiketi ile `<body>` etiketi arasına yerleştirilir.  
Meta veriler genellikle belge başlığını, karakter kümesini, stilleri, komut dosyalarını ve diğer meta bilgileri tanımlar.  
HTML `<head>` öğesi, şu öğeler için bir kapsayıcıdır: `<title>`, `<style>`, `<meta>`, `<link>`, `<script>` ve `<base>`.  
* `<title>`, öğesi, belgenin başlığını tanımlar. Başlık salt metin olmalıdır ve tarayıcının başlık çubuğunda veya sayfanın sekmesinde gösterilir.    
* `<style>`, öğesi, tek bir HTML sayfası için stil bilgilerini tanımlamak için kullanılır.   
* `<link>`, öğesi, geçerli belge ile harici bir kaynak arasındaki ilişkiyi tanımlar. .Çoğunlukla harici stil sayfalarına bağlantı vermek için kullanılır.  
* `<meta>`, öğesi genellikle karakter kümesini, sayfa açıklamasını, anahtar sözcükleri, belgenin yazarını ve görüntü alanı ayarlarını belirtmek için kullanılır.  
* `<script>``, öğesi, istemci tarafı JavaScript'leri tanımlamak için kullanılır.  
* `<base>`, öğesi, bir sayfadaki tüm bağlantılar için bir varsayılan URL ve bir varsayılan hedef belirtir.  
```
<!DOCTYPE html>
<html>
  <head>
    <title>A Meaningful Page Title</title>
    <base href="https://www.w3schools.com/" target="_blank">
    <meta charset="UTF-8">
    <meta name="description" content="Free Web tutorials">
    <meta name="keywords" content="HTML, CSS, JavaScript">
    <meta name="author" content="John Doe">
    <link rel="stylesheet" href="mystyle.css">
    <style>
  	body {background-color: powderblue;}
  	h1 {color: red;}
  	p {color: blue;}
    </style>
    <script>
	function myFunction() {
  	document.getElementById("demo").innerHTML = "Hello JavaScript!";
	}
    </script>
  </head>
  <body>

  </body>
</html>  
```
## Görünümü Ayarlama
Görüntü alanı, kullanıcının bir web sayfasının görünür alanıdır. Cihaza göre değişir - cep telefonunda bilgisayar ekranından daha küçük olacaktır.  
Aşağıdaki <meta> öğesini tüm web sayfalarınıza eklemelisiniz.  
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`  
Bu, tarayıcıya sayfanın boyutlarını ve ölçeklemesini nasıl kontrol edeceğine ilişkin talimatlar verir.  
