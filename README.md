# Ortak-al-masql

Proje Ortakları:
Rauf Agah Subaşı,
Hakan Yalçın,
Gizem Yılmaz

Proje Özeti
Hayvan Hastanesi Otomasyon Sistemi, hayvan hastanesinde çeşitli süreçlerin dijital ortama taşınarak izlenmesi ve yönetilmesini sağlar. Bu sistem, hayvanlar ve sahipleri, veterinerler, randevular, tedavi işlemleri ve hastane içerisindeki diğer operasyonlar gibi birçok işlevsel alanı kapsar. Proje, her bir süreçte tutarlılık ve veri bütünlüğünü sağlarken aynı zamanda verimli bir şekilde bilgiye erişim ve işlem yapma olanağı sunar.
Projede Yer Alacak İşlemler
Randevu Yönetimi: Hayvanlar için randevu oluşturulması, iptal edilmesi ve güncellenmesi işlemlerini içerir.
Tedavi ve Muayene Kaydı: Randevular sonucunda yapılan muayeneler ve tedavi işlemlerinin detaylı kaydının tutulması sağlanır.
İlaç ve Stok Takibi: İlaçların son kullanma tarihine göre takibi, stok durumu ve depolama işlemlerinin yönetimi yapılır.
Fatura Oluşturma ve Takibi: Hayvan sahipleri için tedavi ve diğer hizmetlerin faturalarının oluşturulması ve ödeme durumlarının izlenmesi sağlanır.
Oda ve Konaklama Yönetimi: Hayvanların hastanede konakladığı odaların durumuna göre oda yönetimi yapılır.
Aşı ve Sağlık Takvimi: Hayvanların aşı takvimlerinin düzenlenmesi, yaklaşan aşıların hatırlatılması ve yeni aşıların kaydedilmesi sağlanır.
Beslenme ve Diyet Yönetimi: Hayvanların beslenme planlarının düzenlenmesi ve porsiyon miktarlarının takip edilmesi sağlanır.
Çalışan ve Görev Yönetimi: Çalışanların görev tanımları, iş yükleri ve iletişim bilgilerinin yönetilmesi sağlanır.
Projede Yer Alan Varlıklar ve Nitelikleri
Aşağıda projede kullanılacak başlıca varlıklar ve her bir varlığın sahip olduğu nitelikler verilmiştir:

Hayvanlar: Hayvan hastanesinde tedavi gören her bir hayvanın bilgilerini içerir.

HayvanID, HayvanAdi, Tur, Yas, SahipID, Cinsiyet, Ağırlık, TarihKayit
Sahipler: Hayvanların sahiplerine dair bilgileri içerir.

SahipID, SahipAdi, Telefon, Adres
Veterinerler: Hayvan hastanesinde çalışan veterinerlere ait bilgiler.

VeterinerID, VeterinerAdi, Uzmanlik, Telefon
Randevular: Hayvanlar için alınan randevuların tarih ve saat detaylarını içerir.

RandevuID, HayvanID, VeterinerID, Tarih, Saat, Sorun
Tedaviler: Hayvanlara yapılan tedavilerin kayıtlarını tutar.

TedaviID, RandevuID, TedaviAciklamasi, Ilaclar, TedaviTarihi, Maliyet
İlaçlar: Hayvanların tedavisinde kullanılan ilaçların stok ve son kullanma tarihlerini içerir.

IlacID, IlacAdi, Miktar, SonKullanmaTarihi
Odalar: Hayvanların konakladığı veya tedavi edildiği odaların bilgilerini içerir.

OdaID, OdaAdi, KatNo, Durum
Muayeneler: Yapılan muayene işlemlerinin kayıtları.

MuayeneID, RandevuID, Bulgular, Teshis
Ameliyatlar: Ameliyat geçmişi ve detaylarının tutulduğu tablo.

AmeliyatID, HayvanID, VeterinerID, AmeliyatTarihi, AmeliyatDetaylari, Maliyet
Hastalıklar: Yaygın hastalıklar ve belirtilerini tanımlayan tablo.

HastalikID, HastalikAdi, Belirtiler, TedaviYontemi
Aşılar: Hayvanlara yapılan aşıların takibi için kullanılır.

AsiID, AsiAdi, AsiTarihi, SonrakiAsiTarihi, HayvanID
Faturalar: Hayvan sahiplerinin ödemesi gereken faturaları içerir.

FaturaID, HayvanID, FaturaTarihi, ToplamTutar, OdenmeDurumu
Stoklar: İlaçların depolardaki stok miktarını tutar.

StokID, IlacID, Miktar, DepoYeri
Çalışanlar: Hayvan hastanesinde çalışan personelin bilgilerini içerir.

CalisanID, CalisanAdi, Gorev, Telefon, Maas
Beslenme Planları: Hayvanların beslenme detaylarını tutar.

BeslenmeID, HayvanID, Yemekler, PorsiyonMiktari, OgünSayisi
Laboratuvar Sonuçları: Yapılan test sonuçları ve detayları.

SonucID, HayvanID, TestTarihi, TestAdi, SonucDetayi

![Ekran görüntüsü 2024-11-06 121246](https://github.com/user-attachments/assets/a41b2bca-6935-483a-aacd-14b754e13854)
