# 🚗 Used Cars Price Prediction

* Bu proje, ikinci el araçlara ait teknik özellikler kullanılarak araçların satış fiyatlarının tahmin edilmesi amacıyla geliştirilmiştir.

# 🤖 Kullanılan Model

* AdaBoost Regressor

# 🛠️ Kullanılan Kütüphaneler

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

# 🔄 Yapılan İşlemler

* Veri setinin incelenmesi
* Gereksiz sütunun (`Unnamed: 0`) kaldırılması
* Geçersiz kayıtların (`seats = 0`) veri setinden çıkarılması
* Yinelenen (Duplicate) kayıtların temizlenmesi
* Keşifsel Veri Analizi (EDA)
* Hedef değişken dağılımının incelenmesi
* Aykırı değer analizi
* Kategorik ve sayısal değişken analizleri
* Korelasyon analizi
* Frequency Encoding uygulanması
* One-Hot Encoding uygulanması
* Hedef değişkene (`selling_price`) **Logaritmik Dönüşüm (`log1p`)** uygulanması
* Sayısal değişkenlere **PowerTransformer (Yeo-Johnson)** uygulanması
* Train-Test Split
* AdaBoost Regressor ile model eğitimi
* RandomizedSearchCV ile hiperparametre optimizasyonu
* Farklı veri ön işleme stratejilerinin model performansına etkisinin karşılaştırılması

# 📈 Model Performans Karşılaştırması

| Deney                 | Ön İşleme           | Temel Model R² | Optimize Edilmiş Model R² |
| --------------------- | ------------------- | -------------: | ------------------------: |
| Ön işleme uygulanmadı | -                   |     **62.23%** |                **83.51%** |
| `log1p` dönüşümü      | Hedef değişken      |     **81.57%** |                **89.27%** |
| `PowerTransformer`    | Sayısal değişkenler |     **62.19%** |                **80.22%** |

# 🏆 Sonuç

* Hedef değişkene uygulanan **log1p dönüşümü**, AdaBoost Regressor modelinin performansını belirgin şekilde artırmıştır.
* Sayısal değişkenlere uygulanan **PowerTransformer**, ağaç tabanlı modellerin yapısı gereği model performansında anlamlı bir iyileşme sağlamamıştır.
* En başarılı sonuç, **log1p dönüşümü** ve **hiperparametre optimizasyonu** sonrasında **%89.27 R²** skoru ile elde edilmiştir.

# 📂 Veri Seti

* Kaggle Used Cars Dataset 👉 https://www.kaggle.com/datasets/sukritchatterjee/used-cars-dataset-cardekho

