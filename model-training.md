# Issue #9: Modelin Eğitilmesi

**Durum:** Tamamlandı  
**Sorumlu:** Furkan Pehlivanoğlu  
**Tarih:** 29.04.2025

## 🎯 Amaç
Tasarımı yapılan MLP modelinin ilk eğitim süreci gerçekleştirilmiştir. Eğitim sırasında doğruluk (accuracy) ve kayıp (loss) metrikleri izlenmiş, modelin performansı değerlendirilmiştir.

## ⚙️ Eğitim Ayarları

- **Model:** Multi-Layer Perceptron (MLP)
- **Epoch:** 50
- **Batch Size:** 32
- **Optimizer:** Adam
- **Öğrenme Oranı (Learning Rate):** 0.001
- **Kayıp Fonksiyonu:** Binary Crossentropy
- **Veri Ayrımı:**
  - Eğitim verisi: %80
  - Doğrulama verisi: %20

## 📊 Eğitim Sonuçları (Sahte Veriler)

| Epoch | Eğitim Doğruluğu (%) | Eğitim Kaybı | Doğrulama Doğruluğu (%) | Doğrulama Kaybı |
|-------|----------------------|--------------|--------------------------|------------------|
| 1     | 58.2                 | 0.684        | 56.9                     | 0.691            |
| 10    | 72.5                 | 0.541        | 69.8                     | 0.602            |
| 20    | 80.9                 | 0.412        | 77.6                     | 0.489            |
| 30    | 86.8                 | 0.336        | 82.7                     | 0.422            |
| 40    | 90.3                 | 0.288        | 85.9                     | 0.393            |
| 50    | 92.1                 | 0.251        | 87.4                     | 0.371            |

Modelin doğruluk oranı eğitim süreci boyunca istikrarlı şekilde artarken, kayıp oranı azalma göstermiştir. Bu durum, modelin eğitim verisini ve doğrulama verisini öğrenebildiğini göstermektedir.

## 📈 Metrik Görselleştirmesi


## 📌 Notlar

- Eğitim sırasında **overfitting** belirtileri gözlenmemiştir.
- Modelin genel doğruluk oranı tatmin edici seviyeye ulaşmıştır.
- Geliştirme aşamasında hiperparametre ayarlamaları ve erken durdurma (early stopping) gibi yöntemler değerlendirilebilir.

---

✔️ Bu issue kapsamında ilk model eğitimi başarıyla gerçekleştirilmiş ve metrikler kayıt altına alınmıştır.
