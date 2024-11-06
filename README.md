# Ortak-al-masql
SQL projemiz için ortak çalışma reposudur.
--CREATE TABLE Hayvanlar (
--    HayvanID INT PRIMARY KEY,
--    HayvanAdi VARCHAR(100),
--    Tur VARCHAR(50),
--    Yas INT,
--    SahipID INT, -- Sahibi belirlemek için
--    Cinsiyet VARCHAR(10),
--    Ağırlık DECIMAL(5,2),
--    TarihKayit DATE
--);

--CREATE TABLE Sahipler (
--    SahipID INT PRIMARY KEY,
--    SahipAdi VARCHAR(100),
--    Telefon VARCHAR(15),
--    Adres VARCHAR(255)
--);



--CREATE TABLE Veterinerler (
--    VeterinerID INT PRIMARY KEY,
--    VeterinerAdi VARCHAR(100),
--    Uzmanlik VARCHAR(100),
--    Telefon VARCHAR(15)
--);


--CREATE TABLE Randevular (
--    RandevuID INT PRIMARY KEY,
--    HayvanID INT,
--    VeterinerID INT,
--    Tarih DATE,
--    Saat TIME,
--    Sorun VARCHAR(255),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID),
--    FOREIGN KEY (VeterinerID) REFERENCES Veterinerler(VeterinerID)
--);

--CREATE TABLE Tedaviler (
--    TedaviID INT PRIMARY KEY,
--    RandevuID INT,
--    TedaviAciklamasi VARCHAR(255),
--    Ilaclar VARCHAR(255),
--    TedaviTarihi DATE,
--    Maliyet DECIMAL(10,2),
--    FOREIGN KEY (RandevuID) REFERENCES Randevular(RandevuID)
--);



--CREATE TABLE Ilaclar (
--    IlacID INT PRIMARY KEY,
--    IlacAdi VARCHAR(100),
--    Miktar INT,
--    SonKullanmaTarihi DATE
--);

--CREATE TABLE Odalar (
--    OdaID INT PRIMARY KEY,
--    OdaAdi VARCHAR(50),
--    KatNo INT,
--    Durum VARCHAR(20) -- (Boş, Dolu, Temizlikte vs.)
--);

--CREATE TABLE Muayeneler (
--    MuayeneID INT PRIMARY KEY,
--    RandevuID INT,
--    Bulgular VARCHAR(255),
--    Teshis VARCHAR(255),
--    FOREIGN KEY (RandevuID) REFERENCES Randevular(RandevuID)
--);

--CREATE TABLE Ameliyatlar (
--    AmeliyatID INT PRIMARY KEY,
--    HayvanID INT,
--    VeterinerID INT,
--    AmeliyatTarihi DATE,
--    AmeliyatDetaylari VARCHAR(255),
--    Maliyet DECIMAL(10,2),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID),
--    FOREIGN KEY (VeterinerID) REFERENCES Veterinerler(VeterinerID)
--);


--CREATE TABLE Hastaliklar (
--    HastalikID INT PRIMARY KEY,
--    HastalikAdi VARCHAR(100),
--    Belirtiler VARCHAR(255),
--    TedaviYontemi VARCHAR(255)
--);

--CREATE TABLE Asilar (
--    AsiID INT PRIMARY KEY,
--    AsiAdi VARCHAR(100),
--    AsiTarihi DATE,
--    SonrakiAsiTarihi DATE,
--    HayvanID INT,
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);


--CREATE TABLE Faturalar (
--    FaturaID INT PRIMARY KEY,
--    HayvanID INT,
--    FaturaTarihi DATE,
--    ToplamTutar DECIMAL(10,2),
--    OdenmeDurumu VARCHAR(20), -- (Ödendi, Ödenmedi)
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);

--CREATE TABLE Stoklar (
--    StokID INT PRIMARY KEY,
--    IlacID INT,
--    Miktar INT,
--    DepoYeri VARCHAR(50),
--    FOREIGN KEY (IlacID) REFERENCES Ilaclar(IlacID)
--);

--CREATE TABLE Calisanlar (
--    CalisanID INT PRIMARY KEY,
--    CalisanAdi VARCHAR(100),
--    Gorev VARCHAR(100),
--    Telefon VARCHAR(15),
--    Maas DECIMAL(10,2)
--);

--CREATE TABLE BeslenmePlanlari (
--    BeslenmeID INT PRIMARY KEY,
--    HayvanID INT,
--    Yemekler VARCHAR(255),
--    PorsiyonMiktari DECIMAL(5,2),
--    OgünSayisi INT,
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);



--CREATE TABLE Ziyaretler (
--    ZiyaretID INT PRIMARY KEY,
--    HayvanID INT,
--    ZiyaretciAdi VARCHAR(100),
--    ZiyaretTarihi DATE,
--    ZiyaretNedeni VARCHAR(255),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);


--CREATE TABLE LaboratuvarSonuclari (
--    SonucID INT PRIMARY KEY,
--    HayvanID INT,
--    TestTarihi DATE,
--    TestAdi VARCHAR(100),
--    SonucDetayi VARCHAR(255),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);

--CREATE TABLE Raporlar (
--    RaporID INT PRIMARY KEY,
--    HayvanID INT,
--    VeterinerID INT,
--    RaporTarihi DATE,
--    RaporAciklamasi VARCHAR(255),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID),
--    FOREIGN KEY (VeterinerID) REFERENCES Veterinerler(VeterinerID)
--);

--CREATE TABLE IsYonetimi (
--    IsID INT PRIMARY KEY,
--    CalisanID INT,
--    Gorev VARCHAR(100),
--    BaslangicTarihi DATE,
--    BitisTarihi DATE,
--    IsDurumu VARCHAR(20), -- (Tamamlandı, Devam Ediyor vs.)
--    FOREIGN KEY (CalisanID) REFERENCES Calisanlar(CalisanID)
--);


--CREATE TABLE BeslemeKayitlari (
--    KayitID INT PRIMARY KEY,
--    HayvanID INT,
--    Tarih DATE,
--    Yemek VARCHAR(100),
--    PorsiyonMiktari DECIMAL(5,2),
--    Notlar VARCHAR(255),
--    FOREIGN KEY (HayvanID) REFERENCES Hayvanlar(HayvanID)
--);
--alter table Sahipler add constraint chcksahip foreign key(HayvanID) references Hayvanlar(HayvanID)
--alter table Hastaliklar add  constraint chckhastalik foreign key(HayvanID) references Hayvanlar(HayvanID)
--alter table Odalar add  constraint chckoda foreign key (HayvanID) references Hayvanlar (HayvanID)

