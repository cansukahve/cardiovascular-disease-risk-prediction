# Sağlık Verisiyle Kalp Hastalığı Risk Tahmini

Bu proje, kardiyovasküler hastalık riskini bireylerin demografik ve sağlık verilerini kullanarak tahmin etmeyi amaçlayan bir makine öğrenmesi çalışmasıdır.

---

## 📄 Proje Özeti

Bu çalışmada, Kaggle'dan alınan Kardiyovasküler Hastalık Veri Seti kullanılarak çeşitli veri temizleme, keşifsel veri analizi (EDA) ve modelleme teknikleri uygulanmıştır. Amaç, erken teşhis ve önleyici sağlık önlemleri için bir karar destek sistemi prototipi oluşturmaktır.

### 🎯 Proje Hedefleri
- Kalp-damar hastalığı riskini tahmin eden bir sınıflandırma modeli oluşturmak.
- Risk faktörlerini belirleyip hangi değişkenlerin en etkili olduğunu raporlamak.
- Analiz ve model sonuçlarını Power BI panoları ile görselleştirmek.

---

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler
- **Python 3.12**
- **Pandas & NumPy:** Veri manipülasyonu ve temizliği
- **Matplotlib & Seaborn:** Veri görselleştirme (Jupyter Notebook)
- **Scikit-learn:** Makine öğrenmesi modelleri (Lojistik Regresyon, Random Forest)
- **XGBoost:** Yüksek performanslı sınıflandırma modeli
- **Power BI:** İnteraktif pano (dashboard) oluşturma

---

## 📂 Proje Yapısı
- `data/`: Ham ve temizlenmiş veri setlerini içerir.
- `notebooks/`: Analizin yapıldığı Jupyter Notebook dosyasını içerir.
- `powerbi/`: Power BI rapor dosyalarını içerir.
- `presentation/`: Nihai sunum dosyasını içerir.

---

## 📊 Bulgular ve Sonuçlar

### Keşifsel Veri Analizi (EDA)
- Kolesterol, yaş ve sistolik kan basıncı (ap_hi) gibi değişkenlerin kalp hastalığı riski ile pozitif bir korelasyon gösterdiği tespit edilmiştir.
- Veri seti, hasta ve sağlıklı bireyler açısından dengeli bir dağılıma sahiptir (%49.5'e %50.5).

### Modelleme Sonuçları
- Lojistik Regresyon, Random Forest ve XGBoost modelleri karşılaştırılmıştır.
- En yüksek performansı **%73 doğruluk (accuracy)** oranı ile **XGBoost** modeli göstermiştir.

![Özellik Önem Grafiği](https://i.ibb.co/L95j1bF/feature-importance.png) 
*(Not: Bu kısma, Python'da oluşturduğun özellik önem grafiğinin ekran görüntüsünü yükleyip linkini ekleyebilirsin. Örneğin, [ibb.co](https://tr.imgbb.com/) gibi bir siteye yükleyip linkini alabilirsin.)*

- Modelimize göre, kalp hastalığı riskini belirleyen en önemli üç faktör sırasıyla:
  1.  **Büyük Tansiyon (ap_hi)**
  2.  **Kolesterol**
  3.  **Yaş**

---

## 🚀 Kurulum ve Kullanım

Projeyi kendi bilgisayarınızda çalıştırmak için:
1. Bu repoyu klonlayın: `git clone https://github.com/cansukahve/cardiovascular-disease-risk-prediction.git`
2. `notebooks/` klasöründeki Jupyter Notebook'u açın.
3. Gerekli kütüphaneleri yükleyin: `pip install pandas scikit-learn xgboost matplotlib seaborn`
