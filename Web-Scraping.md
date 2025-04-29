Issue #4: Web Scraping Scriptinin Yazılması
Durum: Tamamlandı
Sorumlu: Furkan Yazgan

Açıklama:
Belirlenen veri kaynaklarından Trendyol Süper Lig futbolcularına ait geçmiş maç performans verilerini çekmek amacıyla Python tabanlı bir web scraping scripti başarıyla geliştirilmiştir. Script, veri çekme işlemlerini hızlı, güvenli ve sistematik bir şekilde gerçekleştirecek şekilde tasarlanmıştır.

Scraping sürecinde Python’ın BeautifulSoup, Requests ve gerekli görülen yerlerde Selenium gibi kütüphaneleri kullanılmıştır. Sayfa yapılarının dinamik özellik göstermesi durumunda Selenium ile tarayıcı simülasyonu gerçekleştirilmiş, statik veri erişiminde ise Requests ve BeautifulSoup yeterli olmuştur.

Scriptin temel işlevleri şunlardır:

Belirlenen oyuncu profili ve maç istatistikleri sayfalarına otomatik erişim,

İlgili sayfalardan oyuncu performans verilerinin (gol, asist, pas başarı oranı, şut sayısı, top kapma, kart bilgileri vb.) doğru şekilde ayrıştırılması,

Elde edilen verilerin temizlenmesi ve yapısal bir formata (örneğin CSV veya JSON) dönüştürülmesi,

Hatalara ve bağlantı sorunlarına karşı hata yakalama ve tekrar deneme mekanizmalarının kurulması,

Gerektiğinde scraping işlemlerinin belirli aralıklarla (örneğin haftalık) otomatik olarak tetiklenebilmesi için temel zamanlayıcı entegrasyonu yapılmıştır.

Script, kaynak sitelerin kullanım politikalarına uyum sağlamak adına aşırı yüklenmeyi önleyici zamanlama (delay), kullanıcı-agent rotasyonu ve temel hız limiti önlemleri ile desteklenmiştir.

Sonuç olarak, belirlenen veri kaynaklarından veri çekimini otomatikleştiren web scraping scripti başarıyla tamamlanmış ve proje için kullanılabilir hale getirilmiştir. İlerleyen aşamalarda verilerin doğrudan veri tabanına aktarılması ve güncelleme mekanizmalarının entegrasyonu planlanmaktadır.