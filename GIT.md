# Get Started
* `git --version` => Git versiyonunu kontrol eder.  
* `git help` => Git ile ilgili bilgiler barındıran yardım rehberi döndürür.  

# Configuring Git
* `git config --global user.name <name>` => Git kullanıcı adı belirlemeye yarar.  
* `git config --global user.email <email>` => Git email adresini belirlemeye yarar.  
* `git config --global --list` => Konfigurasyon ayarlarını görüntülemeye yarar.  

# Setting Up Git Repositories
* `git init` => Local'de bir Git reposu oluştur.  
* `git clone <url>` => Uzak sunucuda bulunan bir Git deposunu local dizine kopyalamayı sağlar.
* `git clone <url> <folder-name>` => Uzak sunucuda bulunan bir Git deposunu localde belirtilen klasöre kopyalamayı sağlar.  
* `git remote -v` => Uzak sunucunun URL bilgisini gösterir.  
* `git remote show <remote-name>` => Spesifik bir uzak sunucunun bilgisini görmeyi sağlar.
* `git remote rm <remote-name>` => Mevcut bir uzak sunucudaki repoyu silmeyi sağlar.  
* `git fetch <remote-name>` => Uzak sunucuda yer alan repoyu getirir ama merge etmez.  
* `git pull <remote-name> <branch-name>` => Komutunu verdiğimizde adını yazdığımız branchda yapılan değişiklikleri localimize çekeriz.

# Managing File Changes
* `git add *` => Tüm yeni ve değiştirilen dosyaları hazırlama alanına ekleyin.
* `git status` => Durumu kontrol et.
* `git diff` => Commit edilmemiş değişiklikleri görebiliriz.
* `git commit -m "açıklama gir"` => Add komutu ile hazırlanan değişiklikler, bir mesaj ile birlikte Local'de ki repository'e kaydedilir.
* `git commit -a -m "commit_mesajı"` => Stagged olmayan ama değişiklik yapılan tüm dosyaları staged yapar ve bir mesaj ile commit atmış olur.

# Review History
* `git log` => Gerçekleştirilen tüm commitleri görmeyi sağlar.
* `git log --since = <date>` => Belirli bir tarihten sonra yapılan commitleri gösterir.

# Branch & Merge
* `git branch -a` => Tüm brachleri listele (Local ve Remote)
* `git checkout <branch_name>` => Belirtilen branc'e geçiş yap.
* `git checkout -b <branch_name>` => Localimizde yeni bir branch oluştururuz ve o branch'a geçiş yapar.
* `git push -u <remote_adı> <branch_name>` => Değişiklikleri uzak repoya aktarır.







