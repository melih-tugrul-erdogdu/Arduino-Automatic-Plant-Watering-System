# 🌱 Arduino Automatic Plant Watering System / Otomatik Bitki Sulama Sistemi
Fransızca anlatımlı proje videosu : https://youtube.com/shorts/vhjwoos76hg
Project video narrated in French : https://youtube.com/shorts/vhjwoos76hg

**TR:** Bu proje, Arduino kullanılarak geliştirilmiş, toprak nemini sürekli izleyen ve kuruluk seviyesi belirlenen eşiğin altına düştüğünde otomatik sulama yapan bir gömülü sistem projesidir.

**EN:** This project is an embedded system developed using Arduino that continuously monitors soil moisture and automatically activates the watering mechanism when the dryness level drops below a specified threshold.

## 📷 Proje Kurulumu / Project Setup

**TR:** Sistem prototipi; sensörler, su pompası ve Arduino'nun entegrasyonu ile kurulmuştur.  
**EN:** The system prototype is set up with the integration of sensors, water pump, and Arduino.

## 🛠 Donanım Bileşenleri / Hardware Components

**TR:** Projede kullanılan temel bileşenler şunlardır:
* **Arduino Uno:** Ana kontrolcü (Microcontroller).
* **Toprak Nem Sensörü (Soil Moisture Sensor):** Toprağın iletkenliğini ölçerek nem verisi sağlar.
* **Su Pompası (Mini Water Pump):** Bitkiyi sulamak için suyu aktarır.
* **Röle Modülü (Relay Module):** Düşük voltajlı Arduino sinyali ile yüksek akım çeken pompayı kontrol eder.
* **Güç Kaynağı ve Kablolar:** Sistemin enerji ihtiyacını karşılar.

**EN:** The main components used in the project are:
* **Arduino Uno:** Main microcontroller.
* **Soil Moisture Sensor:** Provides moisture data by measuring soil conductivity.
* **Mini Water Pump:** Transfers water to irrigate the plant.
* **Relay Module:** Controls the high-current pump using low-voltage Arduino signals.
* **Power Supply & Jumpers:** Powers the system connectivity.

## 💻 Algoritma ve Kod Mantığı / Algorithm & Code Logic

**TR:** Projenin orijinal kaynak kod dosyaları arşivlenmemiştir, ancak çalışma mantığı aşağıdaki ekran görüntüsünde görüldüğü gibidir. Sistem `analogRead` ile veri okur ve `950` eşik değerine göre karar verir.

**EN:** The original source code files are not archived, but the operating logic is preserved in the screenshot below. The system reads data via `analogRead` and makes decisions based on a threshold value of `950`.

### Çalışma Mantığı / How it Works:
1.  **TR:** Sensör topraktan analog veri okur (0-1023). / **EN:** Sensor reads analog data from soil (0-1023).
2.  **TR:** Eğer değer 950'den küçükse (Toprak Kuru), Röle açılır ve Pompa çalışır. / **EN:** If value is < 950 (Soil Dry), Relay turns ON and Pump starts.
3.  **TR:** Eğer değer 950'den büyükse (Toprak Nemli), Pompa durur. / **EN:** If value is > 950 (Soil Wet), Pump stops.

---
**Author/Yazar:** Melih Tuğrul Erdoğdu
