
<img width="1024" height="765" alt="image" src="https://github.com/user-attachments/assets/17c82956-1ce5-49fe-9125-9a6641271ddc" />


## 📍 İçindekiler

1.  [AŞAMA 1: PLANLAMA & YÖNLENDİRME (Strateji ve Güvenlik)](#aşama-1-planlama--yönlendirme-strateji-ve-güvenlik)
    * [OpSec Güvenliği (Teknik)](#-opsec-güvenliği-teknik)
    * [Etik Sınırlar ve Yasal Çerçeve](#️-etik-sınırlar-ve-yasal-çerçeve)
2.  [AŞAMA 2: BİLGİ TOPLAMA (Ham Veri Edinme)](#aşama-2--bilgi-toplama-ham-veri-edinme)
    * [Arama ve Sızıntı Analizi](#-arama-ve-sızıntı-analizi)
    * [Sosyal Medya İstihbaratı (SOCMINT)](#️-sosyal-medya-istihbaratı-socmint)
    * [Teknik Altyapı Taraması](#-teknik-altyapı-taraması)
    * [Alan Adı ve DNS Geçmişi](#-alan-adı-ve-dns-geçmişi)
    * [Kurumsal İstihbarat (Business/Corporate INT)](#-kurumsal-istihbarat-businesscorporate-int)
    * [Resmi Kayıt İstihbaratı (Public Records INT)](#️-resmi-kayıt-istihbaratı-public-records-int)
    * [Web Arşivleme](#-web-arşivleme)
    * [Görüntü Tersine Arama (IMINT)](#️-görüntü-tersine-arama-imint)
    * [Coğrafi Veri Toplama (GEOINT)](#-coğrafi-veri-toplama-geoint)
    * [Havacılık İstihbaratı (AVINT)](#️-havacılık-istihbaratı-avint)
    * [MARINT (Denizcilik İstihbaratı)](#-marint-denizcilik-istihbaratı)
    * [FININT (Finansal İstihbarat) & Kripto OSINT](#-finint-finansal-istihbarat--kripto-osint)
    * [SIGINT (Sinyal İstihbaratı - Halka Açık Yönü)](#-sigint-sinyal-istihbaratı---halka-açık-yönü)
3.  [AŞAMA 3: İŞLEME & DEĞERLENDİRME (Veriyi Ayıklama)](#aşama-3-⚙️-işleme--değerlendirme-veriyi-ayıklama)
4.  [AŞAMA 4: ANALİZ & ÜRETİM (Noktaları Birleştirme)](#aşama-4--analiz--üretim-noktaları-birleştirme)
    * [Ustalık Seviyesi: Analitik Metodoloji](#️-ustalık-seviyesi-analitik-metodoloji-en-kritik-adım)
    * [Bilişsel Yanlılıklar (Cognitive Biases) ve Yönetimi](#-bilişsel-yanlılıklar-cognitive-biases-ve-yönetimi)
    * [Yapılandırılmış Analitik Teknikler (SATs)](#️-yapılandırılmış-analitik-teknikler-sats)
5.  [AŞAMA 5: YAYIM (Raporlama)](#aşama-5--yayim-raporlama)

✷ 　 　　˚ * ✷ 　 　　 　 ·
 　 ˚ *  ⋆ ＊　 　 · 　 ✧　﹡
 　 　　 *　　 * ⋆ 　 .
 · 　　 ⋆ 　⋆ ✧　 　 · 　 ＊　﹡ ˚ ˚ 　　              ˚ *                      ⋆ ＊　 　 ·       *
 　 ⋆ · 　 *        ⋆  *
 　　 ⋆        ﹡　 　    · 　 ✧　˚ *
---


# 0'dan Uzmanlığa TÜRKÇE OSINT Rehberi!

**İstihbarat Döngüsü ve Uygulama Aşamaları**
Hazırlayan: MèSaKu 
Katkıları için  Laox'a teşekkürler.

---

## AŞAMA 1: PLANLAMA & YÖNLENDİRME (Strateji ve Güvenlik)

Görev hedeflerinin netleştirildiği, gerekli kaynakların belirlendiği, etik sınırların çizildiği ve operasyonel güvenliğin (OpSec) sağlandığı stratejik başlangıç aşamasıdır.



### 👻 OpSec Güvenliği (Teknik)
Operasyonel Güvenlik, görevin temel taşıdır. Kimliği (IP, dijital iz) gizlemek için VPN, sanal makineler (VM), güvenli tarayıcılar ve görev için özel oluşturulmuş sahte (sock puppet) profillerin kullanılmasını kapsar.

* **👾 Sanalizasyon ve Ayrıştırma:** Kişisel bilgisayardan izole bir ortamda (`Tails`, `Whonix`, `Kali`) araştırma yapmak için `VirtualBox` veya `VMware` kullanımı.
* **🕸️ Gizli Arama:** `DuckDuckGo`, `Brave Search`, `Firefox` veya `Tor Browser` gibi gizliliğe odaklı tarayıcı ve arama motorları.
* **Geçici E-posta:** Sahte profiller oluşturmak için `temp-mail` gibi geçici e-posta servisleri.

### ⚖️ Etik Sınırlar ve Yasal Çerçeve
Araştırmanın "kırmızı çizgilerini" (hangi bilgilerin toplanıp toplanmayacağını) belirlemek. Özel hayatın gizliliğine ve yerel/uluslararası yasalara (KVKK, GDPR vb.) uymak kritiktir.


---

## AŞAMA 2: 🎣 BİLGİ TOPLAMA (Ham Veri Edinme)

### ☣️ Arama ve Sızıntı Analizi
* **OSINT Framework (osintframework.com):** Bir toplama aracı değil, belirli bir hedef için hangi aracın veya veri kaynağının kullanılacağını gösteren devasa bir dizin ve yol haritasıdır. Görevin kapsamını belirlemek için kullanılır. Alternatif olarak "https://bellingcat.gitbook.io/toolkit" burayı kullanabilirsiniz.
* **Google Dork:** Gelişmiş arama operatörleriyle gizli dosya, veritabanı ve sızıntıları bulma. "https://exposingtheinvisible.org/guides/google-dorking/" Örnek kullanımlar için göz atabilirsiniz.
* **Sızıntı Veritabanları:** `Dehashed`, `HaveIBeenPwned`, `LeakCheck.io`, `IntelligenceX`.
* **Dark Web Taraması:** `.onion` siteleri ve yeraltı forumlarındaki sızıntı ve çalıntı verilerin taranması (`Tor Browser` gerektirir).

🚩 *Not: Bu araçlar yalnızca halka açık verileri analiz eder. Erişim her zaman etik ve yasal sınırlar içinde olmalıdır.*



### 🕵️ Sosyal Medya İstihbaratı (SOCMINT)
Sosyal medya profillerinden ve ağlarından (arkadaş listeleri, beğeniler, etiketlenmiş fotoğtaflar, paylaşımlar) ham veri toplama.

* **Kullanıcı Adı Taraması:** `Sherlock`, `Maigret`, `WhatsMyName` (Kullanıcı adlarını birçok platformda tarar).
* **Telefon Numarası Analizi:** `PhoneInfoga`, `getcontact`, `caller.id` (Telefon numarasından operatör, ülke ve sosyal medya bağlantılarını bulur).
    * *Not: `getcontact` ve `caller.id` gibi ücretli servisler, isim/telefon/geçmiş adres gibi detaylı kişisel kayıtlar sunabilir.*
* **Yüz Arama:** `FaceCheck.id` (Yüz fotoğrafından diğer sosyal medya profillerini veya benzer görüntüleri bulur).
* **Otomatize Arama:** `Seekr-OSINT` (Reddit, Telegram, X gibi platformlarda otomatize arama) ve `SpiderFoot` (Bir hedef için birçok kaynaktan otomatik veri toplar ve ilişkileri haritalar).
    * *Not: SpiderFoot'un `sfp_google`, `sfp_bing`, `sfp_twitter`, `sfp_facebook` gibi modülleri; sızdırılmışsa telefon rehber kayıtlarını, hesap bilgilerini ve sosyal medya profillerini doğrudan getirebilir.*
* **Meta İçerik Kütüphanesi:** Meta'nın Facebook ve Instagram verilerine (öncelikli akademik) erişim aracı.



### 📡 Teknik Altyapı Taraması
* **Altyapı Tespiti:** `Whois` (Alan adı sahiplik bilgisi).
* **Cihaz/Servis Tarama:** `Shodan`, `Censys` (İnternete bağlı cihazları, portları ve servisleri tarar).
    * *Shodan Filtreleri İpucu:*
        * Ülke: `country "ÜLKE KODU"`
        * Şehir: `city "Şehir Adı" country:"ÜLKE KODU"`
        * Koordinat: `geo:"ENLEM,BOYLAM", "KM-ARALIĞI"` (Koordinatı Google Haritalar URL'sinden alabilirsiniz. Ülke kodları için: [nationsonline.org](https://www.nationsonline.org/oneworld/country_code_list.htm))
* **Teknoloji Tespiti:** `Wappalyzer` (eklenti) (Web sitesinin kullandığı teknolojileri [sunucu, CMS, analiz araçları] tespit eder).


### 🔗 Alan Adı ve DNS Geçmişi
Bir web sitesinin geçmişte hangi IP/sunucularda barındığını veya hangi teknolojileri kullandığını görmek.

* **Sunucu Geçmişi:** `Netcraft`.
* **DNS Kayıtları:** `DNSDumpster`, `SecurityTrails` (Geçmiş DNS kayıtları ve alt alan adları).
* **DNS Sorgusu:** `nslookup` (Ters DNS [PTR] sorguları).



### 🏦 Kurumsal İstihbarat (Business/Corporate INT)
Şirket yapılarını, kilit personeli, e-posta formatlarını ve mali durumu araştırmak.

* **Personel ve Yapı:** `LinkedIn (Sales Navigator)`, `Crunchbase`.
* **E-posta Kalıpları:** `Hunter.io`, `Snov.io`.
* **E-posta Doğrulama:** `holehe` (E-posta adreslerinin hangi platformlarda kayıtlı olduğunu kontrol eder).



### 🏛️ Resmi Kayıt İstihbaratı (Public Records INT)
Devletler, belediyeler veya resmi kurumlar tarafından tutulan halka açık kayıtları (dava dosyaları, tapu kayıtları, patentler, ticari markalar, siyasi bağışlar) araştırmak.

* **Araçlar:** Ulusal/yerel mahkeme portal siteleri, tapu ve kadastro veritabanları, patent ofisi arama motorları (örn: `Google Patents`), resmi gazeteler.
* **Kişi Arama Motorları (People Search):** `Pipl`, `Intelius`, `People Finder` hizmetleri.



### ⏳ Web Arşivleme
* **Araçlar:** `Wayback Machine`, `Archive.today` (Silinmiş veya değiştirilmiş web sayfalarının geçmiş sürümlerine erişim sağlar).




### 👁️ Görüntü Tersine Arama (IMINT)
* **Araçlar:** `Google Lens`, `TinEye`, `Yandex Images`, `Bing Images`, `PhotoSherlock` (Görselin kaynağını veya benzerlerini bulur).
    * *İpucu: "Reverse Image Search" gibi tarayıcı eklentileri bu servisleri tek tıkla kullanabilir.*



### 🎯 Coğrafi Veri Toplama (GEOINT)
* **Analiz:** Fotoğraf ve videolardaki ipuçlarından (gölgeler, mimari, trafik işaretleri) çekim yerini tespit etmek.
* **Canlı Kameralar / Wi-Fi:** `Insecam.org`, `Shodan` (webcam filtresi), `Wigle.net` (Dünya çapında Wi-Fi ağ haritaları).
* **Araçlar:** `Geospy Google Earth Studio`, `Google Earth Pro` (Cetvel ve Zaman Aracı), `SunCalc.org` (gölge analizi), `PeakVisor` (dağ/tepe tespiti), `MapDevelopers (Draw Circle Tool)`.
    * *İpucu: `MapDevelopers` veya `Google Earth Pro` ile belirli bir geo-koordinat etrafında (örn. 5km yarıçaplı) bir daire çizerek arama alanını daraltma pratiği yapın.*
    * ** Lokasyon bulmak için ` GeoGuessr ` Oyunu ile pratik yapabilirsiniz. Mükemmeldir!!!



### 🛰️ Havacılık İstihbaratı (AVINT)
* **Uçuş Takibi:** `Flightradar24`, `FlightAware`, `ADS-B Exchange` (Gerçek zamanlı veya geçmiş uçuş hareketleri, rotalar ve sahiplik bilgileri).
* **Rotalar / Tasarımlar:** `Airlineroutemaps.com`, `Airlinersgallery.smugmug.com` (Havayolu rota haritaları ve uçak kuyruk tasarımları).



### ⚓ MARINT (Denizcilik İstihbaratı)
Küresel tedarik zincirini ve gemi hareketlerini (AIS verileri) takip etmek.
* **Araçlar:** `MarineTraffic`, `VesselFinder`, `FleetMon` (Gemilerin konumu, rotası, sahipliği ve yük durumu).



### ₿ FININT (Finansal İstihbarat) & Kripto OSINT
Siber suç ve dolandırıcılık analizlerinde paranın (özellikle kripto paranın) takip edilmesi.

* **Blockchain Gezginleri:** `Etherscan` (Ethereum), `Blockchair`, `BlockCypher`.
* **Cüzdan Analizi:** `Wallet Explorer` (İşlem geçmişlerini ve cüzdanların bilinen borsalarla ilişkisini analiz eder).



### 📶 SIGINT (Sinyal İstihbaratı - Halka Açık Yönü)
Halka açık radyo frekanslarını, uydu sinyallerini ve IoT cihaz iletişimini izlemek.

* **Araçlar:** `SDR (Software Defined Radio)` donanımları, `RadioReference.com` (frekans veritabanları), `Cel-Mapper` (baz istasyonu konumları).

---



## AŞAMA 3: ⚙️ İŞLEME & DEĞERLENDİRME (Veriyi Ayıklama)

* **Metadata Analizi:** `ExifTool` (Fotoğraf, video ve dokümanlardan EXIF verilerini [tarih, saat, GPS konumu, cihaz modeli] okur, işler veya siler).
* **Video Doğrulama:** `InVID`, `WeVerify` (Videolardan meta veri çıkarır, karelere ayırır [tersine arama için] ve manipülasyon [deepfake] tespiti sağlar).
* **Veri Temizleme:** `OpenRefine` (Büyük miktarda metin, sızıntı veya tablo verisini temizler, çift kayıtları siler ve formatları birleştirerek analize hazırlar).

---



## AŞAMA 4: 🧩 ANALİZ & ÜRETİM (Noktaları Birleştirme)

İşlenmiş bilgileri birleştirme, hipotezler kurma, varsayımları sorgulama ve sonuca ulaşma aşaması. **Ustalık bu aşamada kazanılır.**

* **Bağlantı Analizi:** `Maltego`, `Obsidian.md` (Farklı veri noktalarını [kişi, e-posta, şirket, IP] birleştirip aralarındaki gizli ilişkileri görselleştirir).
* **Coğrafi Konum Analizi:** `ipinfo.io`, `iplocation.net` (IP adresinden coğrafi konum çıkararak analizi derinleştirme).
* **Veri Yönetimi:** `CherryTree` (Toplanan verileri birleştirmek için gelişmiş bir not defteri).
* **Zaman Çizelgesi Analizi (Timeline Analysis):** Toplanan tüm verileri (sosyal medya paylaşımları, web sitesi güncellemeleri, uçuş kayıtları) kronolojik bir sıraya dizerek olayların akışını anlama ve örüntüleri ortaya çıkarma.
* **Yapay Zeka ile Fikir Üretme:** Toplanan ham verileri özetlemek, ilişkileri sorgulamak veya potansiyel saldırı senaryoları oluşturmak için `GPT`, `Gemini`, `DeepSeek` gibi yapay zeka araçlarından faydalanma.


### 🎖️ Ustalık Seviyesi: Analitik Metodoloji (En Kritik Adım)
Araçlar veriyi toplar, ancak "Usta" analist o veriden doğru sonucu çıkarır. Bu, beynimizin bize kurduğu tuzakları (Bilişsel Yanlılıklar) bilmekle başlar.



#### 🎭 Bilişsel Yanlılıklar (Cognitive Biases) ve Yönetimi
Analizdeki en büyük düşman, analistin kendi beynidir. Amaç, *Doğrulama Ön Yargısı* (Confirmation Bias - sadece kendi hipotezimizi doğrulayan kanıtları aramak) ve *Çıpalama* (Anchoring - ilk öğrenilen bilgiye takılıp kalmak) gibi analitik tuzakları aktif olarak engellemektir.



#### 🛠️ Yapılandırılmış Analitik Teknikler (SATs)
Bilişsel yanlılıkları yenmek ve karmaşık verileri işlemek için kullanılan standartlaşmış düşünme metodolojileridir. Amaç, hipotezleri test etmek ve varsayımları sorgulamaktır.

* **Örnek Teknikler:**
    * **ACH (Analysis of Competing Hypotheses):** En olası senaryoyu bulmak için kanıtları tüm hipotezlere karşı sistemli bir şekilde puanlama tekniği. (Amaç, en az yanlış olanı bulmaktır.)
    * **Devil's Advocacy (Şeytanın Avukatlığı):** Mevcut ana hipotezi çürütmek için aktif olarak karşı kanıtlar aramak.
    * **Indicators / Signposts (Göstergeler):** Belirli bir hipotezin doğru olup olmadığını anlamak için gelecekte izlenmesi gereken spesifik olayları veya veri noktalarını belirlemek.




---

## AŞAMA 5: 📄 YAYIM (Raporlama)

Sonuçları bir karar vericiye (müşteri, yönetici, okuyucu) net, anlaşılır, kanıta dayalı ve eyleme geçirilebilir bir formatta (rapor, sunum, brifing) sunma aşamasıdır.

* **Modern OSINT Uygulamaları:** Veri çekme, işleme ve görselleştirme için `Python` (Jupyter Notebooks), `R` veya `API'ler` kullanarak süreçleri otomatize etme ve tekrarlanabilir raporlar üretme.

---

### Bilgilendirme

Burada önerilen tüm kaynaklar, yöntemler ve araçlar bilgilendirme amaçlıdır. Bunları daha detaylı öğrenmek için kendi araştırmanızı yapınız.

OSINT konusunda gelişmek istiyorsanız, alternatif senaryoları incelemeli, uygulamalı ve daha derin araştırmalar yapmalısınız.
