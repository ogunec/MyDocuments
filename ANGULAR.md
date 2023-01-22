# Angular Kurulumu
1. Angular CLI çalıştırmak için önce Node.JS kur.
2. Node.JS kurulduktan sonra CMD'ye `npm install -g @angular/cli` komutunu gir.
3. CMD'ye `ng version` komutunu girdiğimizde Angular sürümü çıkıyorsa yükleme başarılı olmuştur.

# Angular Komutları
* `ng version` komutu Angular sürümünü gösterir.
* `ng help` komutu Angular'da kullanabileceğimiz komutların listesini getirir.
* `ng new proje-ismi` komutu ile yeni bir Angular projesi oluşturabiliriz.
* `ng serve` komutu ile oluşturduğumuz projeyi ayağa kaldırırız.
* `ng build` komutu ile uygulamayı build edebiliriz.

# Proje Yapılanması
* __node_modules:__ Uygulamada kullanılan paketler bu dizinde yer alır.
* __src:__ Uygulama ile ilgili çalışmalarımızın %99'u bu klasörde gerçekleşecektir.
* __assets:__ Uygulama ile ilgili resim, video ve icon vs gibi dosyalar bu klasörde yer alır.
* __index.html:__ Temel geliştirme sayfasıdır. Uygulama'da kurgulanacak Single Page burasıdır.
* __main.ts:__ Uygulamanın başlangıç dosyasıdır. .NET'de ki Program.cs'in muadilidir. Hangi modülün ana modül olacağı burada belirtilir.
* __editorconfig:__ Editörle ilgili temel konfigurasyonlar burada gerçekleştirilir.
* __angular.json:__ Uygulamayla ilgili script,style, budgets vs gibi temel konfigurasyonların yapıldığı yer.
* __package-lock.json:__ Uygulamada kullanılan paketlerin sürümleri hakkında bilgiler içerir.
* __tsconfig.json:__ TypeScript ile ilgili konfigurasyonları barındıran dosyadır.
* __app:__ İçerisinde uygulamada kullanılacak componentleri ve diğer Angular yapıtaşlarını barındıracak klasör.
* __app-routing.module.ts:__ Uygulamada sayfalar arası route bilgilerini konfigure ettiğimiz modül dosyası.
* __app.component.html:__ Uygulamada kullanılan ana componentin html dosyası.
* __app.component.ts:__ Ana componentin kodlama dosyası.
* __app.module.ts:__ Uygulamanın ana/root modülü.

# Angular Temel Yapıtaşları
|                   Angular Mimarisinin Temel Yapıtaşları            |
| -------------------- | -------------------- | -------------------- |
| Components           | Data Binding         | Templates            |
| Directives           | Decorators           | Metadatas            |
| Modules              | Services             | Guards               |
| Dependency Injection | Pipes                |                      |
