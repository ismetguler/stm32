# 🚀 STM32 & Gömülü Sistemler Yolculuğum

Burası benim STM32 ile olan maceramın toplandığı yer. Sıfırdan başlayıp, roket aviyoniğine kadar giden yolda öğrendiğim, denediğim ve geliştirdiğim kodları burada biriktiriyorum. Amacım sadece kod yazmak değil; donanımın nasıl çalıştığını, sensörlerin dilini ve gerçek zamanlı sistemleri (RTOS) derinlemesine kavramak.

---

## 🛠️ Neler Kullanıyorum?

* **Kart:** STM32F407VGT6 (Discovery Kit) 
* **Dil:** C (Embedded C)
* **Ortam:** STM32CubeIDE
* **Kütüphane:** HAL (Hardware Abstraction Layer) ama gerektiğinde Register'a da girerim. :)
* **Diğer:** Wokwi, FreeRTOS, Proteus

---

## 📂 Burada Neler Bulacaksınız?

Bu repodaki klasörler benim öğrenme sürecimi kronolojik olarak yansıtıyor. En temelden başlayıp, adım adım daha karmaşık sistemlere geçiyorum.

Genel olarak şunları kurcaladım:
* **Temel Giriş/Çıkış:** LED yakıp söndürmekten, buton okuma ve "Interrupt" (Kesme) mantığına kadar donanımla ilk temas.
* **Analog Dünya (ADC & PWM):** Potansiyometre okuma, motor sürme sinyalleri ve nefes alan LED efektleri.
* **Haberleşme (UART, I2C, SPI):** Sensörlerle konuşma, bilgisayara veri basma ve modüller arası iletişim.
* **Algoritmalar:** Sensör verilerini anlamlandırma ve karar verme mekanizmaları.
* **Gerçek Zamanlı Sistemler (RTOS):** (Şu an üzerinde çalışıyorum) İşlemciye aynı anda birden fazla iş yaptırma sanatı.

---

## 🌟 Göz Bebeği Projem: Sanal Roket Aviyoniği 🚀

Bu repodaki en sevdiğim işlerden biri (`08_Virtual_Rocket`). 
Elimde sensör yokken bile kodla bir "Sanal Roket" simülasyonu oluşturdum. Bu sistem:
1.  Roketin hayali irtifasını hesaplıyor.
2.  Belirli yüksekliğe gelince **otonom karar verip** paraşüt açıyor (LED yakıyor).
3.  Tüm uçuş verilerini anlık olarak bilgisayara (Yer İstasyonuna) raporluyor.
