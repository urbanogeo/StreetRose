![StreetRose](https://github.com/user-attachments/assets/8bdc2ceb-fd6c-4578-bc74-82097ef3232b)

**StreetRose**, OpenStreetMap (OSM) verilerini kullanarak sokak ağı yönelimlerini analiz etmek ve görselleştirmek için yapay zeka desteğiyle tasarlanmış bir kentsel analiz aracıdır. Python ile inşa edilen ve ChatGPT gibi büyük dil modellerinden (LLM'ler) yararlanan StreetRose, gül diyagramları aracılığıyla sokak yönlülüğünün çıkarılmasını, hesaplanmasını ve görselleştirilmesini otomatikleştirir. Araç, hem manuel hem de otomatik veri işleme modları sağlayarak şehirlerle ve sokak morfolojisiyle ilgilenen araştırmacılar bir çözüm sunar.

 **StreetRose** is an urban analysis tool designed with artificial intelligence support to analyze and visualize street network orientations using OpenStreetMap (OSM) data. Built in Python and leveraging large language models (LLMs) such as ChatGPT, StreetRose automates the inference, computation and visualization of street directionality through rose diagrams. The tool provides both manual and automatic data processing modes, offering a solution for researchers interested in cities and street morphology.

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
 

## Features

- **Visual Analysis**: Visualization of street orientations with rose diagrams.
- **Data Integration**: OpenStreetMap data import and manual data entry support.
- **Statistical Analysis**: Calculation of circular statistics such as average orientation, concentration and circular variance.
- User Friendly Interface**: Intuitive and interactive graphical user interface.

## Getting Started

#### Requirements

- Python 3.7 or newer
- The following Python libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scipy`
  - `osmnx`
    
## How does it work?

StreetRose processes street routing data in two modes:

## 1. Manual Mode

-The user loads street network data from an Excel file.

-The tool uses the start and end coordinates of the streets (x1, y1, x2, y2).

-Calculates street directions using trigonometric functions.

-The results are visualized in a rose diagram.

-Users can customize the diagram and export the results.

## 2. OSM Based Mode

-Users specify a region (for example, a city or a neighborhood).

-The vehicle retrieves road network data using OSMnx.

-Street segment directions are calculated based on graph edges.

-The data is processed and analyzed in a geospatial format.

-A rose diagram with statistical summaries is created.


#### Installation

1. **Clone the Warehouse**:
   ```bash
   git clone https://github.com/urbanogeo/StreetRose.git
   cd StreetRose
