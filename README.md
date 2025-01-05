# Hayvan Hastanesi Otomasyon Sistemi Projesi

### Proje Ortakları
- **Rauf Agah Subaşı** (235260133)
- **Hakan Yalçın** (235260139)
- **Gizem Yılmaz** (235260193)

---

## Proje Özeti

Hayvan Hastanesi Otomasyon Sistemi , hayvan hastanesindeki çeşitli süreçlerin dijital ortamda izlenmesi ve yönetilmesini sağlayan bir sistemdir. Bu sistem, hayvanlar ve sahipleri, veterinerler, randevular, tedavi işlemleri ve diğer operasyonel süreçleri kapsar. Sistemin temel amacı, her süreçte tutarlılık ve veri bütünlüğünü sağlarken, bilgiye erişimi ve işlem yapmayı verimli hale getirmektir.

---

## Projede Yer Alacak İşlemler

1. **Randevu Yönetimi**: Hayvanlar için randevu oluşturma, iptal etme ve güncelleme işlemleri.
2. **Tedavi ve Muayene Kaydı**: Randevular sonucunda yapılan muayenelerin ve tedavi işlemlerinin detaylı kaydının tutulması.
3. **İlaç ve Stok Takibi**: İlaçların son kullanma tarihine göre takibi, stok durumu ve depolama işlemleri.
4. **Fatura Oluşturma ve Takibi**: Tedavi ve diğer hizmetler için hayvan sahiplerine fatura oluşturulması ve ödeme durumlarının izlenmesi.
5. **Oda ve Konaklama Yönetimi**: Hayvanların hastanede konakladığı odaların durumuna göre yönetim sağlanması.
6. **Aşı ve Sağlık Takvimi**: Hayvanların aşı takvimlerinin düzenlenmesi, yaklaşan aşıların hatırlatılması ve yeni aşıların kaydedilmesi.
7. **Beslenme ve Diyet Yönetimi**: Hayvanların beslenme planlarının ve porsiyon miktarlarının takip edilmesi.
8. **Çalışan ve Görev Yönetimi**: Çalışanların görev tanımları, iş yükleri ve iletişim bilgilerinin yönetilmesi.

---

## Projede Yer Alan Varlıklar ve Nitelikleri

### Hayvanlar
Hayvan hastanesinde tedavi gören her bir hayvanın bilgilerini içerir.
- **HayvanID**: Hayvanın benzersiz kimliği
- **HayvanAdi**: Hayvanın adı
- **Tür**: Hayvanın türü
- **Yaş**: Hayvanın yaşı
- **SahipID**: Hayvan sahibinin kimliği
- **Cinsiyet**: Hayvanın cinsiyeti
- **Ağırlık**: Hayvanın ağırlığı
- **TarihKayit**: Kayıt tarihi

### Sahipler
Hayvanların sahiplerine dair bilgileri içerir.
- **SahipID**: Sahip kimliği
- **SahipAdi**: Sahip adı
- **Telefon**: İletişim numarası
- **Adres**: İkamet adresi

### Veterinerler
Hastanede çalışan veterinerlere ait bilgileri içerir.
- **VeterinerID**: Veteriner kimliği
- **VeterinerAdi**: Veteriner adı
- **Uzmanlık**: Uzmanlık alanı
- **Telefon**: İletişim numarası

### Randevular
Hayvanlar için alınan randevuların tarih ve saat detaylarını içerir.
- **RandevuID**: Randevu kimliği
- **HayvanID**: Hayvan kimliği
- **VeterinerID**: Veteriner kimliği
- **Tarih**: Randevu tarihi
- **Saat**: Randevu saati
- **Sorun**: Randevu nedeni

### Tedaviler
Hayvanlara yapılan tedavilerin kayıtlarını tutar.
- **TedaviID**: Tedavi kimliği
- **RandevuID**: İlgili randevu kimliği
- **TedaviAçıklaması**: Tedavi detayları
- **İlaçlar**: Kullanılan ilaçlar
- **TedaviTarihi**: Tedavi tarihi
- **Maliyet**: Tedavi maliyeti

### İlaçlar
Tedavide kullanılan ilaçların bilgilerini içerir.
- **İlaçID**: İlaç kimliği
- **İlaçAdi**: İlaç adı
- **Miktar**: Mevcut stok miktarı
- **SonKullanmaTarihi**: Son kullanma tarihi

### Odalar
Hayvanların konakladığı odaların bilgilerini içerir.
- **OdaID**: Oda kimliği
- **OdaAdi**: Oda adı
- **KatNo**: Oda kat numarası
- **Durum**: Oda durumu

### Muayeneler
Yapılan muayene işlemlerinin kayıtlarını içerir.
- **MuayeneID**: Muayene kimliği
- **RandevuID**: İlgili randevu kimliği
- **Bulgular**: Muayene bulguları
- **Teşhis**: Muayene sonucu teşhis

### Ameliyatlar
Ameliyat geçmişi ve detaylarını içerir.
- **AmeliyatID**: Ameliyat kimliği
- **HayvanID**: Hayvan kimliği
- **VeterinerID**: Ameliyatı yapan veteriner kimliği
- **AmeliyatTarihi**: Ameliyat tarihi
- **AmeliyatDetayları**: Ameliyat detayları
- **Maliyet**: Ameliyat maliyeti



### Aşılar
Hayvanlara yapılan aşıların takibini içerir.
- **AşıID**: Aşı kimliği
- **AşıAdi**: Aşı adı
- **AşıTarihi**: Aşı yapılma tarihi
- **SonrakiAşıTarihi**: Sonraki aşı tarihi
- **HayvanID**: İlgili hayvan kimliği

### Faturalar
Hayvan sahiplerinin ödemesi gereken faturaları içerir.
- **FaturaID**: Fatura kimliği
- **HayvanID**: İlgili hayvan kimliği
- **FaturaTarihi**: Fatura tarihi
- **ToplamTutar**: Fatura toplam tutarı
- **ÖdenmeDurumu**: Fatura ödeme durumu







ER DİYAGRAMI



![Ekran görüntüsü 2025-01-05 153631](https://github.com/user-attachments/assets/51ebdbe7-2ffc-42a1-a558-adeb1945ba92)

