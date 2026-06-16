# Mobil Fiyat Sınıflandırma

Bu proje, mobil telefonların fiyat aralığını makine öğrenmesi kullanarak tahmin eder.

## Veri Seti
Veri setinde RAM, batarya gücü, kamera, ekran ve bağlantı özellikleri gibi bilgiler vardır.

## Kullanılan Modeller
- Lojistik Regresyon
- Destek Vektör Makinesi (SVC)
- K-En Yakın Komşu (KNN)

## Yapılan İşlemler
- Veri analizi (EDA)
- Özellik mühendisliği
- Ölçekleme (StandardScaler)
- Model eğitimi
- GridSearchCV ile hiperparametre ayarı
- Model değerlendirme (accuracy, confusion matrix)

## Sonuç
En iyi performansı SVC modeli göstermiştir.

## Kullanılan Kütüphaneler
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
