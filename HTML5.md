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


# HTML Bağlantıları
HTML bağlantıları `<a>` etiketi ile tanımlanır.  

`<a href="https://www.google.com.com">Google</a>`  

Bağlantının hedefi, href niteliği ile belirtilir. Nitelikler, HTML öğeleri hakkında ek bilgi sağlamak için kullanılır.  

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



