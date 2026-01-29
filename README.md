# TikTok Video Classification Project 🎵

## Proje Hakkında
Bu proje, TikTok platformundaki videoları içeriklerine göre **"İddia" (Claim)** veya **"Fikir" (Opinion)** olarak sınıflandıran bir makine öğrenmesi modelidir. Amaç, platformun moderasyon sürecini hızlandırmak ve potansiyel ihlalleri insan incelemesinden önce otomatik olarak tespit ederek iş yükünü azaltmaktır.

Bu çalışma, PACE (Plan, Analyze, Construct, Execute) çerçevesi kullanılarak yapılandırılmıştır.

## 🎯 Hedef
TikTok kullanıcı şikayetlerini ve raporlarını daha verimli yönetebilmek için, videonun bir iddia mı yoksa kişisel bir görüş mü içerdiğini tahmin eden binary classification (ikili sınıflandırma) modeli geliştirmek.

## 🛠️ Kullanılan Teknolojiler
* **Dil:** Python
* **Kütüphaneler:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
* **Modeller:** Random Forest Classifier, XGBoost Classifier
* **NLP:** CountVectorizer (Metin tabanlı özellik çıkarımı için)

## 🚀 Model Performansı
Projede iki ana model eğitilmiş ve karşılaştırılmıştır: **Random Forest** ve **XGBoost**.

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| **Random Forest** | %99+ | %99+ | %99+ | %99+ |
| XGBoost | ~%99 | ~%99 | ~%99 | ~%99 |

* **Sonuç:** Random Forest, hem doğruluk hem de recall (duyarlılık) skorlarında minimal farkla daha iyi performans gösterdiği için nihai model olarak seçilmiştir.

## 📂 Dosya İçeriği
* `TikTok_Classification_Model.ipynb`: Veri analizi, görselleştirme ve model eğitim kodları.
* `tiktok_dataset.csv`: Model eğitimi için kullanılan veri seti.

---
*Bu proje, Google Advanced Data Analytics Sertifika programının bir parçası olarak geliştirilmiştir.*
