# Concrete Strength Prediction

Bu proje, beton karışımında kullanılan malzemelerden yararlanarak **betonun basınç dayanımını (Strength)** tahmin etmek amacıyla geliştirilmiştir.

## Proje Amacı

Gradient Boosting algoritmasında öğrendiğim teorik bilgileri gerçek bir regresyon problemi üzerinde uygulamak ve farklı makine öğrenmesi modellerinin performanslarını karşılaştırmaktır.

## Kullanılan Teknolojiler

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## Veri Seti

Veri seti toplam **1030 gözlem** ve **9 değişkenden** oluşmaktadır.

### Özellikler

* Cement
* Blast Furnace Slag
* Fly Ash
* Water
* Superplasticizer
* Coarse Aggregate
* Fine Aggregate
* Age
* Strength (Hedef Değişken)

## Yapılan Çalışmalar

* Veri inceleme ve temizleme
* Keşifçi Veri Analizi (EDA)
* Korelasyon analizi
* Water/Cement oranı oluşturma
* Gradient Boosting modeli eğitimi
* Hiperparametre optimizasyonu
* Farklı regresyon modelleriyle performans karşılaştırması

## Model Sonuçları

| Model                           |   R² Score |
| ------------------------------- | ---------: |
| Gradient Boosting (Raw Target)  |     89.17% |
| **Gradient Boosting (√Target)** | **91.23%** |
| RandomForestRegressor           |     89.64% |
| DecisionTreeRegressor           |     85.79% |
| AdaBoostRegressor               |     78.84% |
| KNeighborsRegressor             |     74.04% |
| LinearRegression                |     63.83% |
| Ridge                           |     63.76% |
| Lasso                           |     61.51% |
| SVR                             |     56.75% |

## Önemli Bulgular

* Hedef değişkene uygulanan **karekök dönüşümü**, Gradient Boosting modelinin performansını artırmıştır.
* **Ağaç tabanlı modeller** (Gradient Boosting, Random Forest, Decision Tree), doğrusal modellere göre daha başarılı sonuçlar vermiştir.
* **Water/Cement oranı** ile beton dayanımı arasında güçlü negatif ve doğrusal olmayan bir ilişki gözlemlenmiştir.


## Sonuç

Bu proje, hedef değişken dönüşümünün ve ağaç tabanlı ensemble modellerinin beton dayanımı tahmini üzerindeki etkisini incelemektedir. En iyi sonuç, **karekök dönüşümü uygulanmış Gradient Boosting modeli ile %91.23 R²** olarak elde edilmiştir.

## 📂 Veri Seti

* Kaggle Concrete Dataset 👉 https://www.kaggle.com/datasets/zain280/concrete-data

  
## Geliştirici

**Siraç Çelebi**

* GitHub: https://github.com/sirac-celebii
* LinkedIn: https://www.linkedin.com/in/siraccelebii/
