# 🌦️ Szeged (2006–2016) Hava Durumu Analizi

Bu proje, 2006–2016 yılları arasında **Macaristan’ın Szeged şehrine ait hava durumu verilerini** kullanarak  
yağış türünü (**rain**, **snow** veya **none**) makine öğrenmesi ile tahmin etmeyi amaçlamaktadır.  

Veriler gerçek meteorolojik ölçümlerden alınmıştır ve model, sıcaklık, nem, rüzgâr hızı, görüş mesafesi, basınç gibi özellikleri kullanarak  
hangi türde yağış gerçekleşeceğini öngörür.

---

## 📊 Veri Seti Bilgileri

- **Veri Seti Adı:** Weather in Szeged (2006–2016)  
- **Kaynak:** [Kaggle – Weather in Szeged 2006–2016](https://www.kaggle.com/datasets/budincsevity/szeged-weather)  
- **Kapsam:** 2006–2016 yılları arasında Macaristan’ın Szeged şehrinde kaydedilmiş günlük hava durumu ölçümleri.  
- **Veri Sağlayıcısı:** Dark Sky API (artık Apple Weather veritabanına dahil edilmiştir)

### 📋 Sütunlar (Columns)
| Sütun Adı | Açıklama |
|------------|-----------|
| `Formatted Date` | Tarih ve saat bilgisi |
| `Summary` | Havanın kısa özeti (örneğin: *Partly Cloudy*) |
| `Precip Type` | Yağış türü (*rain*, *snow* veya boş) |
| `Temperature (C)` | Sıcaklık (°C) |
| `Apparent Temperature (C)` | Hissedilen sıcaklık (°C) |
| `Humidity` | Nem oranı (0–1 arası) |
| `Wind Speed (km/h)` | Rüzgâr hızı |
| `Visibility (km)` | Görüş mesafesi |
| `Pressure (millibars)` | Hava basıncı |
| `Daily Summary` | Günlük genel hava özeti |

---

## 🎯 Proje Amaçları

1. 2006–2016 yılları arasında Szeged’deki hava durumu değişimlerini analiz etmek.  
2. Sıcaklık, nem, rüzgâr hızı gibi değişkenler arasındaki ilişkileri incelemek.  
3. Hava durumu ile ilgili halk inanışlarını (folklore) gerçek ölçümlerle karşılaştırmak.  
4. Elde edilen verileri görselleştirerek trendleri ve örüntüleri ortaya çıkarmak.  
5. Basit regresyon veya makine öğrenmesi modelleriyle yağış tipi tahmini yapmak.  

---

## 🧠 Yöntem (Methodology)

1. **Veri Temizleme:**  
   Eksik verilerin doldurulması, tarih formatlarının dönüştürülmesi ve veri tipi hatalarının düzeltilmesi.  

2. **Keşifsel Veri Analizi (EDA):**  
   Sıcaklık, nem, rüzgâr hızı gibi değişkenlerin dağılımlarının incelenmesi.  
   Değişkenler arası korelasyonların heatmap ile gösterilmesi.  

3. **Görselleştirme:**  
   `Matplotlib` ve `Seaborn` kütüphaneleri kullanılarak grafiksel analizlerin yapılması.  

4. **Modelleme (Opsiyonel):**  
   `Scikit-learn` ile regresyon modelleri (Linear Regression, Random Forest vb.) oluşturulabilir.  

---

## 🧰 Kullanılan Teknolojiler

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn** 

---

## 📁 Dosyalar

| Dosya Adı | Açıklama |
|------------|-----------|
| `weatherHistory.csv` | Ham hava durumu verisi |
| `calisma.ipynb` | Analiz ve grafiklerin bulunduğu Jupyter Notebook |
| `README.md` | Proje açıklama dosyası |

---

## 🚀 Nasıl Çalıştırılır

1. Bu repoyu bilgisayarına indir veya klonla:
   ```bash
   git clone https://github.com/<kullaniciadi>/Weather-in-Szeged-2006-2016.git
