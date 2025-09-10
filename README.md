# 🔐 Akıllı Kapı Otomatı – RFID Kart Okuma

Bu proje, **RFID sensörü** kullanarak kapı kartı okuyan ve servo motor aracılığıyla kapıyı açabilen basit, güvenli ve akıllı bir sistem sunar. RFID kart tanımlama ile yalnızca yetkili kişilerin giriş yapabilmesini sağlar.  

## 🚀 Özellikler
- 📡 **RFID Kart Tanıma** (ör. RC522 modülü ile)
- 🔑 **Yetkili Kart Kontrolü** – yalnızca belirlenen UID’ler kapıyı açabilir
- ⚙️ **Arduino Kontrollü Mekanizma** – servo motor veya elektronik kilit entegrasyonu
- 💡 **LED ve Seri Monitör Geri Bildirimi**
- 🛠️ **Kolay Kurulum ve Özelleştirme**

## 🧩 Kullanılan Donanım
- Arduino UNO (veya uyumlu kart)
- MFRC522 RFID Okuyucu Modül
- Servo Motor / Elektronik Kilit
- LED (opsiyonel – görsel bildirim için)
- Breadboard ve jumper kablolar

  <img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/6cc76aaa-d81a-44dd-bf9a-d58918f29b0b" />


## 📥 Kurulum
1. Repoyu klonla:
   ```bash
   git clone https://github.com/dilaracelik73/Ardunio_Project.git
   cd Ardunio_Project
2. Arduino IDE veya PlatformIO ile .ino dosyasını aç.
3. Gerekli kütüphaneleri yükle:
    MFRC522
    SPI

4. Kendi donanımına göre pin tanımlarını ve kart UID’lerini düzenle.
5. Arduino’nu bilgisayara bağla ve kodu yükle.

🖱️ Kullanım
Sisteme tanımlı bir RFID kart okutulduğunda servo motor çalışır ve kapı açılır.
Tanımsız bir kart okutulduğunda LED kırmızı yanar ve seri monitörden uyarı alınır.

## Tanımlı kart UID listesi
String authorizedUIDs[] = {
  "AB CD EF 12",
  "34 56 78 90"
};

## 📊 Geri Bildirim
- Yeşil LED: Kart tanındı, kapı açıldı ✅
- Kırmızı LED: Yetkisiz kart ❌
- Seri Monitör: Kart UID bilgisi loglanır

## 🖼️ Donanım Bağlantı Şeması
- Aşağıdaki diyagramda Arduino UNO – RC522 RFID – Servo Motor bağlantıları gösterilmektedir:

📌 Not: assets/arduino_rfid_schematic.png dosyasını kendin oluşturup bu dizine eklemelisin. Önerilen araç: Fritzing

## 🔮 Geliştirme Fikirleri
- LCD/OLED ekran ekleyerek giriş bilgisi gösterme
- ESP8266/ESP32 ile Wi-Fi üzerinden uzaktan kontrol
- MQTT ile IoT entegrasyonu
- Web paneli veya mobil uygulama ile kart yönetimi

## 🤝 Katkıda Bulunma
Katkı yapmak istersen:
 -  Bu repoyu fork et
 -  Yeni bir özellik için branch aç
 -  Değişikliklerini commit et
 -  Pull Request gönder 🎉

## 📜 Lisans
MIT License © 2025 Dilara Çelik







