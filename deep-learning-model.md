# Issue #8: Derin Öğrenme Modelinin Tasarlanması

**Durum:** Tamamlandı  
**Sorumlu:** Furkan Pehlivanoğlu  
**Tarih:** 29.04.2025

## 🔍 Amaç
Bu aşamada projemiz için uygun bir derin öğrenme modeli seçilmiş ve katman yapısı detaylandırılmıştır. Projede kullanılan veri tipi ve problemin yapısı göz önüne alınarak **MLP (Multi-Layer Perceptron)** modeli tercih edilmiştir. Modelin sınıflandırma performansını artırmak adına farklı aktivasyon fonksiyonları ve katman kombinasyonları değerlendirilmiştir.

## 🧠 Seçilen Model: Multi-Layer Perceptron (MLP)

MLP modeli, tam bağlantılı (fully connected) katmanlardan oluşur ve genellikle yapısal verilerle çalışan sınıflandırma/regresyon problemlerinde tercih edilir. Bu projede kullanılacak model aşağıdaki şekilde yapılandırılmıştır:

### 🔧 Model Mimarisi

| Katman              | Boyut | Aktivasyon Fonksiyonu |
|---------------------|-------|------------------------|
| Girdi Katmanı       | 128   | -                      |
| Gizli Katman 1      | 64    | ReLU                   |
| Gizli Katman 2      | 32    | ReLU                   |
| Çıkış Katmanı       | 1     | Sigmoid                |

### 🎯 Aktivasyon Fonksiyonları

- **ReLU (Rectified Linear Unit):** Gizli katmanlarda kullanılan yaygın bir aktivasyon fonksiyonudur. Negatif değerleri sıfırlar, pozitif değerleri aynen geçirir.
- **Sigmoid:** Çıkış katmanında tercih edilmiştir çünkü projemiz **binary classification (ikili sınıflandırma)** problemi çözmektedir.

## 📌 Notlar

- Model `Keras` kullanılarak `Sequential` API ile yapılandırılacaktır.
- Daha ileri seviye iyileştirmeler için dropout, batch normalization gibi teknikler ileriki aşamalarda değerlendirilecektir.

---

✔️ Bu issue kapsamında modelin temel mimarisi ve aktivasyon fonksiyonları başarıyla belirlenmiş, uygulanabilir hale getirilmiştir.
