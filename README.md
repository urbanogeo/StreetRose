![StreetRose](https://github.com/user-attachments/assets/8bdc2ceb-fd6c-4578-bc74-82097ef3232b)
 
**StreetRose**, OpenStreetMap (OSM) verilerini kullanarak sokak ağı yönelimlerini analiz etmek ve görselleştirmek için yapay zeka desteğiyle tasarlanmış bir kentsel analiz aracıdır. Python ile inşa edilen ve ChatGPT gibi büyük dil modellerinden (LLM'ler) yararlanan StreetRose, gül diyagramları aracılığıyla sokak yönlülüğünün çıkarılmasını, hesaplanmasını ve görselleştirilmesini otomatikleştirir. Araç, hem manuel hem de otomatik veri işleme modları sağlayarak şehirlerle ve sokak morfolojisiyle ilgilenen araştırmacılar bir çözüm sunar.


## Özellikler

- **Görsel Analiz**: Gül diyagramlarırile sokak yönelimlerinin görselleştirilmesi.
- **Veri Entegrasyonu**: OpenStreetMap verilerinin içe aktarılması ve manuel veri girişi desteği.
- **İstatistiksel Analiz**: Ortalama yönelim, konsantrasyon ve dairesel varyans gibi dairesel istatistiklerin hesaplanması.
- **Kullanıcı Dostu Arayüz**: Sezgisel ve etkileşimli grafik kullanıcı arayüzü.

## Başlarken

### Gereksinimler

- Python 3.7 veya daha yeni bir sürüm
- Aşağıdaki Python kütüphaneleri:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scipy`
  - `osmnx`
    
## Nasıl Çalışır ?

StreetRose sokak yönlendirme verilerini iki modda işler:

## 1. Manuel Mod

-Kullanıcı bir Excel dosyasından sokak ağı verilerini yükler.

-Araç sokakların başlangıç ve bitiş koordinatlarını (x1, y1, x2, y2) kullanır.

-Trigonometrik fonksiyonları kullanarak sokak yönlerini hesaplar.

-Sonuçlar bir gül diyagramında görselleştirilir.

-Kullanıcılar diyagramı özelleştirebilir ve sonuçları dışa aktarabilir.

## 2. OSM Tabanlı Mod

-Kullanıcılar bir bölge belirler (örneğin, bir şehir veya mahalle).

-Araç, OSMnx kullanarak yol ağı verilerini alır.

-Sokak segmenti yönleri grafik kenarlarına göre hesaplanır.

-Veriler jeo-uzamsal bir formatta işlenir ve analiz edilir.

-İstatistiksel özetlerle birlikte bir gül diyagramı oluşturulur.


### Kurulum

1. **Depoyu Klonlayın**:
   ```bash
   git clone https://github.com/urbanogeo/StreetRose.git
   cd StreetRose
