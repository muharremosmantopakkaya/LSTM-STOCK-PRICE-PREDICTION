# LSTM ile Hisse Senedi Fiyat Tahmini

Bu proje, LSTM (uzun kısa vadeli bellek) kullanarak bir hisse senedinin fiyatını tahmin etmeyi amaçlar. 

## Kullanılan Kütüphaneler

- `numpy`: Sayısal işlemler için kullanıldı.
- `pandas`: Veri işleme ve veri yapıları için kullanıldı.
- `matplotlib.pyplot`: Veri görselleştirme için kullanıldı.
- `sklearn.preprocessing.MinMaxScaler`: Veriyi ölçeklendirme için kullanıldı.
- `keras.models.Sequential`, `keras.layers.LSTM`, `keras.layers.Dense`, `keras.layers.Dropout`: Derin öğrenme modeli için kullanıldı.
- `yfinance`: Hisse senedi verilerini çekmek için kullanıldı.
- `ta`: Teknik analiz göstergelerini hesaplamak için kullanıldı.

## Proje Açıklaması

### Hisse Senedi Verisi Alma ve Görselleştirme
Projede, belirli bir hisse senedinin fiyat verileri `yfinance` kütüphanesi kullanılarak çekilmiş ve kapanış fiyatları görselleştirilmiştir.

### Veri Hazırlama
Veri, ölçeklendirilerek LSTM modeline uygun hale getirilmiştir. Eğitim ve test veri setleri oluşturulmuştur.

### LSTM Modeli Oluşturma ve Eğitme
Model, LSTM katmanları, dropout katmanları ve yoğun (dense) katmanlar kullanılarak oluşturulmuş ve eğitilmiştir.

### Tahminler ve Görselleştirme
Model kullanılarak test veri seti üzerinde fiyat tahminleri yapılmış ve gerçek fiyatlarla karşılaştırılmıştır. Elde edilen sonuçlar görselleştirilmiştir.

## Yapılan İşlemler ve Çıktılar

- **Kod Hücresi 1:** Hisse senedi verisinin alınması, görselleştirilmesi, veri hazırlama, LSTM modeli oluşturma ve eğitme adımları bulunmaktadır.
- **Kod Hücresi 2:** Teknik analiz göstergelerinin hesaplanması ve görselleştirilmesi aşamaları içerir.
- **Kod Hücresi 3:** `ta` kütüphanesinin kurulumu ve gereken işlemler yer alır.
- **Kod Hücresi 4:** Başka bir zaman aralığında farklı bir modelleme ve tahmin işlemi gerçekleştirilmiştir.

## Kullanım

1. Proje klasörünü klonlayın:
    ```bash
    git clone https://github.com/muharremosmantopakkaya/LSTM-STOCK-PRICE-PREDICTION.git
    ```
2. Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install -r requirements.txt
    ```
3. Projeyi çalıştırın ve sonuçları gözlemleyin.
