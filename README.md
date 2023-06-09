Merhabalar,

Asp.Net MVC kullanarak Paytr entegrasyonunu başarıyla gerçekleştirdim. İşlem adımlarını aşağıda detaylı bir şekilde açıklıyorum:

İlk olarak, bir form oluşturmanız gerekmektedir. Bu form aracılığıyla kullanıcıdan e-posta, tutar, ad ve soyad gibi verileri alacaksınız. Bunun için HomeController içinde Index ActionResult'ında formu oluşturmalısınız.

Formu dolduran kullanıcılar tarafından gönderilen verileri almak için HomeController içindeki Paytr ActionResult'ına post etmelisiniz. Bu aşamada Paytr'ın sağladığı mağaza verilerini doldurmanız gerekmektedir.

Gerekli verileri doldurduktan sonra Paytr view'ına iframe'i eklemeniz gerekmektedir. Bu iframe, ödeme işlemini Paytr üzerinden gerçekleştirecektir. Örnek olarak Paytr view'ında iframe örneği bulunmaktadır.

Ödeme işlemi Paytr tarafından gerçekleştirildikten sonra, Paytr tarafından post metoduyla gönderilen ödeme verilerini almanız gerekmektedir. Bunun için HomeController içinde Bildirim ActionResult'ını (Hem Get Hem Post metodu olarak) oluşturmalısınız.

Get metodu, yönlendirme yapacağınız alanı belirtirken, Post metodu siparişinizi başarıyla veritabanına kaydetme, mail gönderme gibi işlemleri gerçekleştirmeniz için kullanılır.

Bildirim ActionResult'i, içi boş bir şekilde oluşturmanız gerekmektedir. Sadece ekrana "OK" yazması yeterlidir. Bu sayfa kullanıcı tarafından görüntülenmeyecek, sadece Paytr tarafından bildirim almak için kullanılacaktır.

Paytr bildirimlerini alabilmek için Paytr Mağaza paneline giriş yaptıktan sonra Ayarlar menüsünden Bildirim Url'inin doğru olarak ayarlanması gerekmektedir. Bu bildirim URL'i, oluşturduğunuz Post metodu adresine yönlendirecektir.

Bu şekilde Paytr entegrasyonunu başarıyla gerçekleştirebilirsiniz. İyi çalışmalar dilerim.
