Git VCS (Version Control System) normal şartlar altında lokalde çalışır.

Yani sizin .git klasörüne sahip bir projede yaptığınız güncelleme, aynı .git klasörüne sahip başka bir bilgisayara direkt olarak YANSIMAZ.

Projenin lokalde kalması ekip halinde çalışılan bir projeyi kötü etkiler çünkü herkes yeni bir commit(sürüm) ekledikten sonra projenin ".git" klasörünü diğerleriyle paylaşmak zorunda kalır.


furkan pcsi ".git" klasörü:

> first commit
> style.css güncellendi

esra pcsi ".git" klasörü:

> first commit
> index.html

# Github Bulut Sistemi

Git projelerinin depolanması ve ekip halinde çalışılan projelerin daha sağlıklı güncellenebilmesi için uzun süre boyunca bir bulut sisteme ihtiyaç duyuldu. Bunun üzerine Github adındaki platform ortaya çıktı. Linus Torvalds(Linux geliştiricisi) tarafından oluşturuldu.

Git ortak versiyon kontrol sisteminin adıyken Github bu versiyon kontrol sistemini kullanan projelerin saklanabildiği bir bulut hizmeti ve web sitesidir.

Git eşsizken Github'ın alternatifleri mevcuttur:

>GitLab
>BitBucket

# Remote vs Local

Bilgisayarımızda git init ile oluşturduğumuz projeler lokaldir.
Lokaldeki Git ile internetteki Github arasında bir UZAK BAĞLANTI ihtiyacı duyarız.

Uzak bağlantıları yöneten git komutu "git remote" tur.

origin lakabıyla bir URL belirlememizi sağlayıp her seferinde linki kopyala yapıştır yapmaktan bizi kurtaran komut
buradaki "origin" sadece bu projedeki origindir. Yani şuan bulunduğumuz git projesinin hangi linke yükleneceğini temsil eder.
Her projenin ayrı bir origini(reposu) olduğu için, proje başına bu komutu 1 kere çalıştırmak yeterlidir.

>git remote add origin https://github.com/frknecn4/coffee-project.git

push => yereldeki dosyaların ve versiyonların uzağa(buluta, remote'a) gönderilmesini temsil eder
>git push -u origin frknecn3/css-fix