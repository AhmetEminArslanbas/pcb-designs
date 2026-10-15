<div align="center">

# 🔌 PCB Tasarımları ve 3B Baskı Parçaları

**Altium Designer ile şemasını ve baskı devresini tasarladığım mikrodenetleyici kartları, sensör modülleri, güç ve motor sürücü kartları, ayrıca projelerim için tasarladığım 3B baskı parçaları**

![Altium](https://img.shields.io/badge/Altium%20Designer-A5915F?logo=altiumdesigner&logoColor=white)
![3D](https://img.shields.io/badge/3B%20bask%C4%B1-FDM-orange)

<img src="docs/boards/rp2350-dev-board.jpg" width="720" alt="RP2350 geliştirme kartı">

</div>

## Geliştirme kartları

<table>
<tr>
<td width="50%" valign="top"><img src="docs/boards/rp2350-dev-board.jpg"><br>
<b>RP2350 geliştirme kartı (Pico 2 uyumlu)</b><br>
RP2350A, W25Q32 QSPI flash, RT6150B buck-boost 3,3 V regülatör, USB-C, BOOT/RESET düğmeleri, SWD başlığı, Pico pin düzeni.
</td>
<td width="50%" valign="top"><img src="docs/boards/rp2040-dev-board.jpg"><br>
<b>RP2040 geliştirme kartı</b><br>
RP2040, W25Q16 flash, RT6150B regülatör, USB-C, güç yolu koruması (Schottky + P-MOSFET), Pico pin düzeni.
</td>
</tr>
<tr>
<td width="50%" valign="top"><img src="docs/boards/esp32-dev-board.jpg"><br>
<b>ESP32 geliştirme kartı</b><br>
ESP32-WROOM-32, CP2102N USB-UART, otomatik programlama devresi (transistörlü EN/IO0), AMS1117 3,3 V, USB-C ve ESD koruması.
</td>
<td width="50%" valign="top"><img src="docs/boards/atmega328-nano.jpg"><br>
<b>ATmega328P kartı (Nano uyumlu)</b><br>
ATmega328P, FT232RL USB-UART, 78M05 regülatör, USB-C, durum LED'leri, ICSP başlığı.
</td>
</tr>
</table>

## Modüller ve güç kartları

| | | |
|---|---|---|
| <img src="docs/boards/imu-baro-module.jpg"><br>**IMU + barometre modülü**<br>MPU6050 + BMP280, LD3985 LDO; uçuş bilgisayarları için tek modül | <img src="docs/boards/mpu6050-module.jpg"><br>**MPU6050 modülü**<br>6 eksen IMU, LDO, montaj delikli | <img src="docs/boards/bmp280-module.jpg"><br>**BMP280 modülü**<br>Basınç/irtifa sensörü, I2C/SPI |
| <img src="docs/boards/l298n-motor-driver.jpg"><br>**L298N motor sürücü**<br>Çift H-köprü, flyback diyotları, 78M05 lojik beslemesi | <img src="docs/boards/lm2587-boost.jpg"><br>**LM2587 boost dönüştürücü**<br>Yükseltici DC-DC, Schottky diyot, giriş/çıkış filtreleri | <img src="docs/schematics/lm2596-buck.png"><br>**LM2596 buck dönüştürücü**<br>Düşürücü DC-DC (şema) |

> Görseller Altium kart dosyalarından KiCad 3B görüntüleyicisiyle render edilmiştir. Şema önizlemeleri [`docs/schematics`](docs/schematics) klasöründedir.

## 3B baskı parçaları
Drone, RC araç ve robot projelerim için tasarlayıp FDM yazıcıda bastığım parçalardan bazıları (STL/G-code dosyalarından render):

| | | |
|---|---|---|
| <img src="docs/3d-prints/gear_17t.png"><br>17 dişli çark | <img src="docs/3d-prints/tinywhoop_battery_holder.png"><br>Tiny Whoop pil tutucu | <img src="docs/3d-prints/drone_battery_holder.png"><br>Drone pil tutucu |
| <img src="docs/3d-prints/motor_mount.png"><br>Motor döndürme aparatı | <img src="docs/3d-prints/rc_car_part.png"><br>RC araç parçası | |

## Neler öğrendim
- Mikrodenetleyici kartı tasarımı: kristal ve flash yerleşimi, USB diferansiyel hatları, güç yolu koruması, programlama devreleri.
- Anahtarlamalı güç kaynaklarında (buck/boost) bileşen seçimi ve yerleşimi.
- Kendi kartlarımı ve parçalarımı robot projelerinde kullanarak tasarım–üretim–test döngüsü.

---
<sub>© Ahmet Emin Arslanbaş — Tüm hakları saklıdır. Tasarım dosyaları paylaşılmamıştır.</sub>
