Issue #5: Ham Verinin Temizlenmesi ve Ön İşlenmesi
Bu aşamada ilk olarak elimizdeki ham veriyi inceledim. Verinin içinde eksik değerler (null veya boş olanlar) vardı. Öncelikle bu eksik verileri tespit ettim ve verinin yapısına göre farklı işlemler uyguladım:

Eğer eksik değerler çok fazlaysa o satırı tamamen kaldırdım.
Eğer az sayıda eksik değer varsa, ortalama, medyan gibi yöntemlerle doldurdum.
Ayrıca veri içinde tutarsızlıklar vardı. Örneğin bazı futbolcuların mevkii bilgileri küçük harfle, bazılarının ise büyük harfle yazılmıştı. Bunların hepsini standart hale getirdim (hepsini küçük harf yaptım gibi).
Son olarak tarih, sayı gibi alanlarda da uygun formatları kullandım (örneğin doğum tarihlerini "YYYY-MM-DD" formatına çevirdim). Böylece veri modellemeye hazır hale geldi.

Issue #6: Özellik Mühendisliği (Feature Engineering)
Veriyi temizledikten sonra modele daha iyi sinyal verecek yeni özellikler ürettim.

Örneğin, sadece oynanan maç sayısına bakmak yerine maç başına ortalama gol gibi yeni bir özellik ekledim.
Ya da yaş ve tecrübe süresinden "performans potansiyeli" gibi tahmini bir değişken oluşturdum.
Buradaki amacım, modelin daha iyi öğrenebilmesi için anlamlı ve etkili değişkenler yaratmaktı. Bu süreçte hem temel istatistiklere (ortalama, oran gibi) hem de domain bilgisine (futbol bilgisinden gelen sezgilere) dayandım.
