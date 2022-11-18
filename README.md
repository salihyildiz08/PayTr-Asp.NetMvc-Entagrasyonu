Merhabalar,

Asp .Net Mvc ile Paytr entegrasyon işlemini yaptım.

* Öncelikle bir form ayarlamalısınız.(Email,Tutar,Ad Soyad verileri almak için.)
* HomeController içinde Index ActionResult'da formumu oluşturun.
* Formumdan HomeController içindeki Paytr ActionResult'a verileri post edin.
* Burada gerekli mağaza verileri doldurmanız gerekmektedir.
* Gerekli verileri doldurduktan sonra Paytr view'a iframe'i(örnekteki gibi) yazmanız gerekmektedir.
* Buradaki işlemleri gerçekleştirdikten sonra Paytr tarafından post ile ödeme gerçekleştiği verileri alacaksınız.
* HomeController içinde Bildirim ActionResult'ı oluşturun(Hem Get Hem Post Metodu).
* Get metodu ile oluşturduğunuzu yer sizin yönlendirme yapacağınız alan.
* Post Metodu ile siparişinizi başarıyla veritabanına kaydetme, mail gönderme gibi işlemleri burada yapınız.
* Bildirim ActionResult oluşturmanız gerekiyor. İçi bomboş olmalı ekrana sadece OK yazması gerekmektedir(Kullanılan bir sayfa değildir.).
* Bildirimleri alabilmek için Paytr Mağaza girişi yaptıktan sonra Ayarlar menüsünden Bildirim Url'i doğru yazmanız gerekmektedir(Oluşturulan post metoduna gidecektir.).

Bu şekilde paytr entegrasyonunuz başarıyla gerçekleşmiş olacaktır.

İyi Çalışmalar Dilerim.
