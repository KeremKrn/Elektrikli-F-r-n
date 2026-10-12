# Elektrikli-F-r-n
Etrafı gazbetonlarla yalıtımlı, gömülü rezistans ile ısınan ekranlı ve sıcaklık ayarlanabilir, sıcaklık ölçebilen ve yeterli sıcaklığa gelince otomatik duran bir elektrikli fırın projesi.
-----------------------------------
# Elektrikli Fırın Kontrol Sistemi

Bu proje, meslek lisesi Elektrik-Elektronik Alanı 9. sınıf eğitimi kapsamında geliştirildiğim bir sıcaklık kontrol ve otomasyon çalışmamdır.
Sistem, termokupl ile alınan sıcaklık verisine göre rezistansın SSR röle üzerinden güvenli bir şekilde anahtarlanmasını sağlar.

## Proje Özellikleri ve Çalışma Mantığı
* **Sıcaklık Ölçümü:** MAX6675 termokupl modülü kullanılarak yüksek sıcaklık değerleri okunur.
* **Güç Kontrolü:** Arduino dijital çıkışı ile tetiklenen 25A SSR (Solid State Relay) üzerinden 220V rezistans hattı anahtarlanır.
* **Kullanıcı Arayüzü:** 20x4 LCD ekran ve yön butonları ile sistem durumu takip edilir.
* **Veri Kaydı:** MicroSD kart modülü ile çalışma verileri kaydedilebilir.
* **Soğutma ve Güvenlik:** Kasa içi sıcaklık dengesi için 12V fan ve emniyet şalteri (toggle switch) entegre edilmiştir.

---

## Kullanılan Malzemeler
* Arduino Uno kontrol kartı
* SSR-25DA Solid State Röle (24-380VAC / 25A)
* MAX6675 Termokupl Sensör Modülü
* 20x4 I2C LCD Ekran
* MicroSD Kart Modülü
* Rezistans Teli ve 220V Gösterge Lambası
* 12V Soğutma Fanı ve Adaptör
* SPST Toggle Switch, Butonlar ve 220 Ohm Direnç

---

## Bağlantı Şeması ve Güvenlik Uyarısı
Sistem bağlantı detayları `docs/circuit_diagram.png` dosyasında yer almaktadır. 

---

## Görseller
| Kontrol Kutusu | Fırın Gövdesi |
| :---: | :---: |
| ![Panel](docs/control_panel.jpg) | ![Gövde](docs/furnace_body.jpg) |
