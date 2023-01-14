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

* 
