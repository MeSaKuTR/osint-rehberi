
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
    * [Kurumsal İstihbarat (Business/Corporate INT)](#-kurumsal-istihbaratı-businesscorporate-int)
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
    * [Bilişselyanlılıklar (Cognitive Biases) ve Yönetimi](#-bilişsel-yanlılıklar-cognitive-biases-ve-yönetimi)
    * [Yapılandırılmış Analitik Teknikler (SATs)](#️-yapılandırılmış-analitik-teknikler-sats)
5.  [AŞAMA 5: YAYIM (Raporlama)](#aşama-5--yayim-raporlama)
6.  [ÖNERİLEN KİTAPLAR VE İLERİ OKUMALAR](#📚-önerilen-kitaplar-ve-ileri-okumalar)
7.  [AKADEMİK VAKA ANALİZİ: "OPERASYON: GÖLGE AĞ"](#🎓-akademik-vaka-analizi-operasyon-gölge-ağ)


✷ 　 　　˚ * ✷ 　 　　 　 ·
 　 ˚ *  ⋆ ＊　 　 · 　 ✧　﹡
 　 　　 *　　 * ⋆ 　 .
 · 　　 ⋆ 　⋆ ✧　 　 · 　 ＊　﹡ ˚ ˚ 　　              ˚ *                      ⋆ ＊　 　 ·       *
 　 ⋆ · 　 *        ⋆  *
 　　 ⋆        ﹡　 　    · 　 ✧　˚ *




___




# 0'dan Uzmanlığa TÜRKÇE OSINT Rehberi!

**İstihbarat Döngüsü ve Uygulama Aşamaları** _Hazırlayan: MèSaKu (Katkıları için Laox'a teşekkürler.)_





## AŞAMA 1: PLANLAMA & YÖNLENDİRME (Strateji ve Güvenlik)

Görev hedeflerinin netleştirildiği, gerekli kaynakların belirlendiği, etik sınırların çizildiği ve operasyonel güvenliğin (OpSec) sağlandığı stratejik başlangıç aşamasıdır.




### 👻 OpSec Güvenliği (Teknik)

Operasyonel Güvenlik, görevin temel taşıdır. Kimliği (IP, dijital iz) gizlemek için VPN, sanal makineler (VM), güvenli tarayıcılar ve görev için özel oluşturulmuş sahte (sock puppet) profillerin kullanılmasını kapsar.

-   ** Sanalizasyon ve Ayrıştırma:** Kişisel bilgisayardan izole bir ortamda (`Tails`, `Whonix`, `Kali` vb.) gibi işletim sistemlerinde araştırma yapmak için kendi kişisel bilgisayarınıza kurmak yerine `VirtualBox` veya `VMware`gibi sanal makine kullanımları!
    
-   ** Gizli Arama ve Geniş Arama:** `DuckDuckGo`, `Brave Search`, `Firefox` veya `Tor Browser` gibi gizliliğe odaklı tarayıcı ve arama motorları.

-   **Sahte Profiller:** Basit konular için sahte profiller oluşturmak için `temp-mail` gibi geçici e-posta servisleri.

Ama önemli konularda dikkat çekmemek ve doğal akışta bir istihbarat toplamak için ya kendi sunucunuza bağlı bir mail yada proton gibi üst seviye güvenlikli mail servisleri kullanın!  

- Yapay zeka ile üretilmiş gerçek hayatta olmayan kişi fotoğrafı üretiyor: "ThisPersonDoesNotExist.com" Sahte profillerinizde kullanabilirsiniz..

- **Teknik İlişkilendirmeyi (Attribution) Kırmak:** 

Akıllı hedefler seni sadece IP'nden tanımaz. Seni Tarayıcı da ki parmak İzine odaklanırlar yani(Browser Fingerprint)'nden tanır: Kullandığın yazı tipleri (fonts), ekran çözünürlüğün, tarayıcı eklentilerin... Milyonlarca insan arasında seni "benzersiz" yapan bir imzadır bu.

 - **Nasıl Çözebiliriz:**  KOYUN SÜRÜSÜNE KARIŞACAĞIZ. Dünyada en çok kullanılan çözünürlük, font ve işletim sistemi kullanmak gibi! 
 
 **EK OLARAK**
 
 - Tarayıcılarınızın kendine has özel gizlilik ayarlarını max düzeyde kullanın. Özel ayarlarda var mesela (Firefox'ta privacy.resistFingerprinting) kullanmak vb.
 
 - Güvenilir olmayan kaynaklarda arama yaparken(".onion" uzantılı siteler) tarayıcınızı orjinal (Resolution) çözünürlüğünüzde kullanmaya çalışın! Siteler genelde bunları logluyor...




###  Etik Sınırlar ve Yasal Çerçeve

Araştırmanın "kırmızı çizgilerini" (hangi bilgilerin toplanıp toplanmayacağını) belirlemek. Özel hayatın gizliliğine ve yerel/uluslararası yasalara (KVKK, GDPR vb.) uymak kritiktir.


Teknik İlişkilendirmeyi (Attribution) Kırmak:

## AŞAMA 2:  BİLGİ TOPLAMA (Ham Veri Edinme)


###  Arama ve Sızıntı Analizi

-   **OSINT Framework:** Bir toplama aracı değil, belirli bir hedef için hangi aracın veya veri kaynağının kullanılacağını gösteren devasa bir dizin ve yol haritasıdır.
    
    -   [osintframework.com](https://osintframework.com)
        
    -   Alternatif: [Bellingcat Toolkit](https://bellingcat.gitbook.io/toolkit)
        
-   **Dev Referans GitHub Kaynakları:** Alanında en çok kabul gören ve sürekli güncellenen araç ve kaynak koleksiyonları.
    
    -   [github.com/jivoi/awesome-osint](https://github.com/jivoi/awesome-osint)
        
    -   [github.com/tracelabs/awesome-osint](https://github.com/tracelabs/awesome-osint)
        
    -   [github.com/cipher387/osint\_stuff\_tool\_collection](https://github.com/cipher387/osint_stuff_tool_collection)
        
    -   [github.com/Astrosp/Awesome-OSINT-For-Everything](https://github.com/Astrosp/Awesome-OSINT-For-Everything)
        


-   **Google Dork ve Meta-Arama Motorları:** Gelişmiş arama operatörleriyle gizli dosya, veritabanı ve sızıntıları bulma.
    
    -   Örnek kullanım: [Exposing the Invisible - Google Dorking](https://exposingtheinvisible.org/guides/google-dorking/)

    - `Dogpile` (https://www.dogpile.com/) bir "metasearch engine" yani meta-arama motorudur. Google, Bing, Yahoo gibi birden fazla arama motorunun sonuçlarını birleştirir.
        
-   **Sızıntı Veritabanları:** `Dehashed`, `HaveIBeenPwned`, `LeakCheck.io`, `IntelligenceX`, `Socradar.io`.
    
-   **Dark Web Taraması:** `.onion` siteleri ve yeraltı forumlarındaki sızıntı ve çalıntı verilerin taranması (`Tor Browser` gerektirir).
    


> 🚩 **Not:** Bu araçlar yalnızca halka açık verileri analiz eder. Erişim her zaman etik ve yasal sınırlar içinde olmalıdır.

### 🕵️ Sosyal Medya İstihbaratı (SOCMINT)

Sosyal medya profillerinden ve ağlarından (arkadaş listeleri, beğeniler, etiketlenmiş fotoğraflar, paylaşımlar) ham veri toplama.

-   **Kullanıcı Adı Taraması:** `Sherlock`, `Maigret`, `WhatsMyName` (Kullanıcı adlarını birçok platformda tarar).
    
-   **Twitter (X) Odaklı Analiz:** `Twint` (Gelişmiş Twitter veri çekme/arşivleme aracı), `Followerwonk` (Twitter biyografi analizi ve takipçi karşılaştırma).
    
-   **Telefon Numarası Analizi:** `PhoneInfoga`, `getcontact`, `caller.id` (Telefon numarasından operatör, ülke ve sosyal medya bağlantılarını bulur).
    
    -   > **Not:** `getcontact` ve `caller.id` gibi ücretli servisler, isim/telefon/geçmiş adres gibi detaylı kişisel kayıtlar sunabilir.
        
-   **Yüz Arama:** `FaceCheck.id` (Yüz fotoğrafından diğer sosyal medya profillerini veya benzer görüntüleri bulur).
    
-   **Otomatize Arama:** `Seekr-OSINT` (Reddit, Telegram, X gibi platformlarda otomatize arama) ve `SpiderFoot` (Bir hedef için birçok kaynaktan otomatik veri toplar ve ilişkileri haritalar).
    
    -   > **Not:** SpiderFoot'un `sfp_google`, `sfp_bing`, `sfp_twitter`, `sfp_facebook` gibi modülleri; sızdırılmışsa telefon rehber kayıtlarını, hesap bilgilerini ve sosyal medya profillerini doğrudan getirebilir.
        
-   **Meta İçerik Kütüphanesi:** Meta'nın Facebook ve Instagram verilerine (öncelikli akademik) erişim aracı.
    

###  Teknik Altyapı Taraması

-   **Altyapı Tespiti:** `Whois` (Alan adı sahiplik bilgisi).
    
-   **Recon Çerçeveleri:** `Recon-ng` (Web tabanlı keşif için modüler bir çerçeve), `TheHarvester` (E-postaları, alt alan adlarını, çalışan isimlerini ve portları toplar).
    
-   **Cihaz/Servis Tarama:** `Shodan`, `Censys` (İnternete bağlı cihazları, portları ve servisleri tarar).
    
    -   > **Shodan Filtreleri İpucu:**
        
    -   > Ülke: `country:"ÜLKE KODU"`
        
    -   > Şehir: `city:"Şehir Adı" country:"ÜLKE KODU"`
        
    -   > Koordinat: `geo:"ENLEM,BOYLAM", "KM-ARALIĞI"` (Koordinatı Google Haritalar URL'sinden alabilirsiniz. Ülke kodları için: [nationsonline.org](https://www.nationsonline.org/oneworld/country_code_list.htm))
        
-   **Teknoloji Tespiti:** `Wappalyzer` (eklenti) (Web sitesinin kullandığı teknolojileri \[sunucu, CMS, analiz araçları\] tespit eder).
   
   BuiltWith ise o sitenin tarihsel olarak (geçmişte) hangi teknolojileri (CMS, sunucu, e-posta sağlayıcı, analiz araçları vb.) kullandığını da gösteren devasa bir veritabanıdır. İkisi birbirinin tamamlayıcısı ve en önemli "Teknoloji Tespiti" araçlarıdır. `BuiltWith` (builtwith.com)
   
    
- `Expolit-DB` (https://www.exploit-db.com/) Sistemlerin bilinen zafiyetlerini (exploit) aramak için kullanılır. 

Örneğin önce Shodan, Censys veya Wappalyzer ile bir hedef (sunucu, servis, yazılım) bulursunuz. Sonra, bulduğunuz o yazılımın (örn: "Apache 2.4.51") bilinen bir zafiyeti var mı diye Exploit-DB'ye bakarsınız.



###  Alan Adı ve DNS Geçmişi

Bir web sitesinin geçmişte hangi IP/sunucularda barındığını veya hangi teknolojileri kullandığını görmek.

-   **Sunucu Geçmişi:** `Netcraft`.
    
-   **DNS Kayıtları:** `DNSDumpster`, `SecurityTrails` (Geçmiş DNS kayıtları ve alt alan adları).
    
-   **DNS Sorgusu:** `nslookup` (Ters DNS \[PTR\] sorguları).
    

###  Kurumsal İstihbarat (Business/Corporate INT)

Şirket yapılarını, kilit personeli, e-posta formatlarını ve mali durumu araştırmak.

-   **Personel ve Yapı:** `LinkedIn` (Sales Navigator), `Crunchbase`.
    
-   **E-posta Kalıpları:** `Hunter.io`, `Snov.io`.
    
-   **E-posta Doğrulama:** `holehe` (E-posta adreslerinin hangi platformlarda kayıtlı olduğunu kontrol eder).
    

###  Resmi Kayıt İstihbaratı (Public Records INT)

Devletler, belediyeler veya resmi kurumlar tarafından tutulan halka açık kayıtları (dava dosyaları, tapu kayıtları, patentler, ticari markalar, siyasi bağışlar) araştırmak.

-   **Araçlar:** Ulusal/yerel mahkeme portal siteleri, tapu ve kadastro veritabanları, patent ofisi arama motorları (örn: `Google Patents`), resmi gazeteler.
    
-   **Kişi Arama Motorları (People Search):** `Pipl`, `Intelius`, `People Finder` hizmetleri.
    

###  Web Arşivleme

-   **Araçlar:** `Wayback Machine`, `Archive.today` (Silinmiş veya değiştirilmiş web sayfalarının geçmiş sürümlerine erişim sağlar).
    

###  Görüntü Tersine Arama (IMINT)

-   **Araçlar:** `Google Lens`, `TinEye`,`PimEyes`,`Yandex Images`, `Bing Images`, `PhotoSherlock` (Görselin kaynağını veya benzerlerini bulur).
    
    -   > **İpucu:** "Reverse Image Search" gibi tarayıcı eklentileri bu servisleri tek tıkla kullanabilir.
        

###  Coğrafi Veri Toplama (GEOINT)

-   **Analiz:** Fotoğraf ve videolardaki ipuçlarından (gölgeler, mimari, trafik işaretleri) çekim yerini tespit etmek.
    
-   **Canlı Kameralar / Wi-Fi:** `Insecam.org`, `Shodan` (webcam filtresi), `Wigle.net` (Dünya çapında Wi-Fi ağ haritaları).
    
-   **Araçlar:** `Geospy`, `Google Earth Studio`, `Google Earth Pro` (Cetvel ve Zaman Aracı), `Creepy` (Sosyal medya paylaşımlarından konum verisi toplar), `SunCalc.org` ,`Twilight Map (in-the-sky.org/twilightmap.php)` (gölge analizi). `PeakVisor` (dağ/tepe tespiti), `MapDevelopers` (Draw Circle Tool).

- **Araç Plakaları:** Araç plakalarının hangi ülkeye ait oldduğunu tarihsel olarak depolayan bir database "http://www.worldlicenseplates.com/" 
    
    -   > **İpucu:** `MapDevelopers` veya `Google Earth Pro` ile belirli bir geo-koordinat etrafında (örn. 5km yarıçaplı) bir daire çizerek arama alanını daraltma pratiği yapın.
        
-   **Pratik:** **Lokasyon bulmak için `GeoGuessr` Oyunu ile pratik yapabilirsiniz. Mükemmeldir!!!**
    


###  Havacılık İstihbaratı (AVINT)

-   **Uçuş Takibi:** `Flightradar24`, `FlightAware`, `ADS-B Exchange` (Gerçek zamanlı veya geçmiş uçuş hareketleri, rotalar ve sahiplik bilgileri).
    
-   **Rotalar / Tasarımlar:** `Airlineroutemaps.com`, `Airlinersgallery.smugmug.com` (Havayolu rota haritaları ve uçak kuyruk tasarımları).
    

###  MARINT (Denizcilik İstihbaratı)

Küresel tedarik zincirini ve gemi hareketlerini (AIS verileri) takip etmek.

-   **Araçlar:** `MarineTraffic`, `VesselFinder`, `FleetMon` (Gemilerin konumu, rotası, sahipliği ve yük durumu).
    

### ₿ FININT (Finansal İstihbarat) & Kripto OSINT

Siber suç ve dolandırıcılık analizlerinde paranın (özellikle kripto paranın) takip edilmesi.

-   **Blockchain Gezginleri:** `Etherscan` (Ethereum), `Blockchair`, `BlockCypher`.
    
-   **Cüzdan Analizi:** `Wallet Explorer` (İşlem geçmişlerini ve cüzdanların bilinen borsalarla ilişkisini analiz eder).
    

###  SIGINT (Sinyal İstihbaratı - Halka Açık Yönü)

Halka açık radyo frekanslarını, uydu sinyallerini ve IoT cihaz iletişimini izlemek.

-   **Araçlar:** `SDR (Software Defined Radio)` donanımları, `RadioReference.com` (frekans veritabanları), `Cel-Mapper` (baz istasyonu konumları).
    

## AŞAMA 3:  İŞLEME & DEĞERLENDİRME (Veriyi Ayıklama)

-   **Metadata Analizi:** `ExifTool` (Fotoğraf, video ve dokümanlardan EXIF verilerini \[tarih, saat, GPS konumu, cihaz modeli\] okur, işler veya siler).
    
-   **Video Doğrulama:** `InVID`, `WeVerify` (Videolardan meta veri çıkarır, karelere ayırır \[tersine arama için\] ve manipülasyon \[deepfake\] tespiti sağlar).
    
-   **Veri Temizleme:** `OpenRefine` (Büyük miktarda metin, sızıntı veya tablo verisini temizler, çift kayıtları siler ve formatları birleştirerek analize hazırlar).

-   **Görsel Netleştirme:** `unblur veya deblur` PhotoShop bilginiz yoksa bulanık ve net bilgi elde edilemeyen fotoğrafları netleştirebilirsiniz.
    

## AŞAMA 4:  ANALİZ & ÜRETİM (Noktaları Birleştirme)

İşlenmiş bilgileri birleştirme, hipotezler kurma, varsayımları sorgulama ve sonuca ulaşma aşaması. _Ustalık bu aşamada kazanılır._

-   **Bağlantı Analizi:** `Maltego`, `Obsidian.md` (Farklı veri noktalarını \[kişi, e-posta, şirket, IP\] birleştirip aralarındaki gizli ilişkileri görselleştirir).
    
-   **Coğrafi Konum Analizi:** `ipinfo.io`, `iplocation.net` (IP adresinden coğrafi konum çıkararak analizi derinleştirme).
    
-   **Veri Yönetimi:** `CherryTree` (Toplanan verileri birleştirmek için gelişmiş bir not defteri).
    
-   **Zaman Çizelgesi Analizi (Timeline Analysis):** Toplanan tüm verileri (sosyal medya paylaşımları, web sitesi güncellemeleri, uçuş kayıtları) kronolojik bir sıraya dizerek olayların akışını anlama ve örüntüleri ortaya çıkarma.
    
-   **Yapay Zeka ile Fikir Üretme:** Toplanan ham verileri özetlemek, ilişkileri sorgulamak veya potansiyel saldırı senaryoları oluşturmak için `GPT`, `Gemini`, `DeepSeek` gibi yapay zeka araçlarından faydalanma.
    

### Ustalık Seviyesi: Analitik Metodoloji (En Kritik Adım)

Araçlar veriyi toplar, ancak "Usta" analist o veriden doğru sonucu çıkarır. Bu, beynimizin bize kurduğu tuzakları (Bilişsel Yanlılıklar) bilmekle başlar.

-   **Gerçek OSINT Vaka Analizleri (Nasıl Yapılır):** Analiz tekniklerinin gerçek dünyada nasıl uygulandığını görmek için Bellingcat'in vaka incelemeleri ve "Nasıl yapılır" rehberleri incelenmelidir.
    
    -   [Bellingcat How-Tos](https://www.bellingcat.com/category/resources/how-tos/)
        

###  Bilişsel Yanlılıklar (Cognitive Biases) ve Yönetimi

Analizdeki en büyük düşman, analistin kendi beynidir. Amaç, **Doğrulama Ön Yargısı** (_Confirmation Bias_ - sadece kendi hipotezimizi doğrulayan kanıtları aramak) ve **Çıpalama** (_Anchoring_ - ilk öğrenilen bilgiye takılıp kalmak) gibi analitik tuzakları aktif olarak engellemektir.

###  Yapılandırılmış Analitik Teknikler (SATs)

Bilişsel yanlılıkları yenmek ve karmaşık verileri işlemek için kullanılan standartlaşmış düşünme metodolojileridir. Amaç, hipotezleri test etmek ve varsayımları sorgulamaktır.

-   **Örnek Teknikler:**
    
    -   **ACH (Analysis of Competing Hypotheses):** En olası senaryoyu bulmak için kanıtları tüm hipotezlere karşı sistemli bir şekilde puanlama tekniği. (Amaç, en az yanlış olanı bulmaktır.)
        
    -   **Devil's Advocacy (Şeytanın Avukatlığı):** Mevcut ana hipotezi çürütmek için aktif olarak karşı kanıtlar aramak.
        
    -   **Indicators / Signposts (Göstergeler):** Belirli bir hipotezin doğru olup olmadığını anlamak için gelecekte izlenmesi gereken spesifik olayları veya veri noktalarını belirlemek.
        
-   **Detaylı SATs Makaleleri (Akademik Kaynaklar):**
    
    -   [CIA Tradecraft Primer (PDF)](https://www.cia.gov/resources/csi/static/Tradecraft-Primer-apr09.pdf)
        
    -   [RAND Corporation - Analytic Thinking (PDF)](https://www.rand.org/content/dam/rand/pubs/research_reports/RR1400/RR1408/RAND_RR1408.pdf)
        

## AŞAMA 5: 📄 YAYIM (Raporlama)

Sonuçları bir karar vericiye (müşteri, yönetici, okuyucu) net, anlaşılır, kanıta dayalı ve eyleme geçirilebilir bir formatta (rapor, sunum, brifing) sunma aşamasıdır.

-   **Modern OSINT Uygulamaları:** Veri çekme, işleme ve görselleştirme için `Python` (`Jupyter Notebooks`), `R` veya `API`'ler kullanarak süreçleri otomatize etme ve tekrarlanabilir raporlar üretme.
    

___

##  Önerilen Kitaplar ve İleri Okumalar

**OSINT Techniques: Resources for Uncovering Online Information — Michael Bazzell**

-   Sektördeki en temel ve kapsamlı kaynaklardan biri olarak kabul edilir. Bazzell, yöntemlerini sürekli günceller. (Baskı (2024) itibarıyla ~590 sayfa.)
    

**Open Source Intelligence Methods and Tools: A Practical Guide to Online Intelligence — Nihad A. Hassan & Rami Hijazi**

-   2018’de yayınlanmış, OSINT döngüsünün her aşaması için pratik araçlar ve yöntemler sunan güçlü bir rehber.
    

**Deep Dive: Exploring the Real-world Value of Open Source Intelligence — Rae L. Baker**

-   2023’te yayınlanmış bu kitap, OSINT’in modern ve güncel yönlerini, özellikle kurumsal dünyadaki değerini ele alır.



___

 
 ## **SİZE ÇOĞU DİSİPLİNİ İÇEREN GÜZEL BİR SENARYO OLUŞTURDUM.**

 ### Senaryo: "Operasyon: Gölge Ağ" (Akademik Vaka Analizi)

**Hedef:** "Ph03nix\_7" kod adlı kurgusal bir tehdit aktörünün kimliğini, operasyonel konumunu ve para aklama yöntemlerini, birden fazla istihbarat disiplinini (IMINT, MARINT, FININT, Teknik INT) çapraz doğrulayarak (cross-corroborate) tespit etmek.

**Başlangıç Kanıtları:**

1.  **Persona:** `Ph03nix_7` (Dark Web forum kullanıcı adı)
    
2.  **Görsel Kanıt:** Hedefin Twitter'da paylaştığı tek bir fotoğraf. Mesaj: "Another day at the office..." Fotoğraf, bir pencereden görünen _belirsiz_ bir liman/sahil şeridi manzarası içeriyor.
    
3.  **Finansal İz:** Fidye için kullanılmış (artık terk edilmiş) bir Bitcoin (BTC) cüzdan adresi.
    

___

### Analiz Aşamaları ve Kullanılan Uzman Araçları

**1\. Aşama: Keşif ve Görüntü Analizi (IMINT & Automation)**

Analist, `Ph03nix_7` personasını haritalamak için **`SpiderFoot`** gibi bir otomasyon çerçevesi başlatır. Paralel olarak, fotoğrafa odaklanır:

-   **IMINT (Görsel Arama):** Fotoğraftaki belirsiz liman manzarası **`Google Lens`** veya **`Yandex Images`** ile aratılır. Sonuçlar geneldir (binlerce liman fotoğrafı) ve spesifik bir konum (GEOINT) **tespit edilemez.** Bu, analistin coğrafi konum için başka bir yol bulması gerektiği anlamına gelen ilk "çıkmaz sokak"tır.
    
-   **IMINT (Meta Veri Analizi):** Fotoğraf **`ExifTool`** ile analiz edilir: `exiftool Ph03nix_tweet.jpg`
    
-   **BULGU (Pivot 1):** Twitter, GPS ve kamera modeli gibi verilerin çoğunu temizlemiştir. Ancak, `Date/Time Original` (Orijinal Tarih/Saat) meta verisi korunmuştur: **`2024-10-26 14:30:12`**. Analist bu zaman damgasını (timestamp) kritik bir veri olarak not eder.
    

**2\. Aşama: Pivot Noktası (Google Dorking & Tehdit İstihbaratı)**

GEOINT'in başarısız olması nedeniyle dijital ayak izleri daha da kritik hale gelir. Analist, hedefin geçmişteki OpSec hatalarını bulmak için **`Google Dorking`** kullanır.

-   Spesifik bir dork (`intext:"Ph03nix_7" "gmail.com" site:pastebin.com`) yıllar önce paylaşılan bir kod dökümünü (paste) ortaya çıkarır.
    
-   **BULGU (Pivot 2):** Kodun yorum satırında `# Author: James Hawkins <james.hawkins.dev@gmail.com>` bilgisi bulunur. Persona artık gerçek bir kimlikle ilişkilendirilmiştir.
    
-   Bu e-posta adresi, **`IntelligenceX`** gibi derin bir tehdit istihbaratı arşivinde aratılır. Bir veri sızıntısında (`MyFitnessPal`) bu e-postayla birlikte kaydedilen tarihsel bir IP adresi (`81.149.x.x`) bulunur.
    

**3\. Aşama: Altyapı ve Kurumsal Doğrulama (Passive DNS & Corporate INT)**

Analist, bulunan IP ve ismi doğrulamak için altyapı araçlarına yönelir:

-   IP adresi, **`SecurityTrails`** (veya `RiskIQ PassiveTotal`) gibi bir Pasif DNS platformunda analiz edilir. IP'nin tarihsel kayıtlarının olmaması, bunun bir sunucu değil, "Londra" konumlu bir ev interneti (Residential ISP) olduğunu teyit eder.
    
-   "James Hawkins" ismi, `LinkedIn` ve **`theHarvester`** kullanılarak 'SecureData Solutions Ltd.' adlı bir şirketle ilişkilendirilir.
    
-   Analist, **`Offshore Leaks Database`** (ICIJ) veya ilgili ülkenin (örn. Kıbrıs, BVI) **Resmi Ticaret Sicili** (Corporate Registry) kayıtlarını inceler.
    
-   **BULGU (Pivot 3):** "James Hawkins"in bu şirketin kurucu yöneticisi olduğu ve şirketin resmi adresinin **"Limassol Marina, Kıbrıs"** olduğu tespit edilir.
    

**4\. Aşama: "WOW" Anı - Çapraz Doğrulama (IMINT + GEOINT + MARINT)**

Bu, senaryonun akademik zirvesidir. Analistin elinde iki ayrı, bağımsız ve _doğrulanmamış_ veri vardır:

1.  **Fotoğraftan (Adım 1):** Zaman Damgası: `26 Ekim 2024, 14:30:12`
    
2.  **Resmi Kayıtlardan (Adım 3):** Konum: `Limassol Marina, Kıbrıs`
    

-   **Hipotez:** James Hawkins, 26 Ekim saat 14:30'da Limassol Marina'daki ofisindeydi ve o fotoğrafı çekti.
    
-   **Test (Denizcilik İstihbaratı - MARINT):** Analist, **`MarineTraffic`** platformunu açar.
    
-   **Eylem:** "Playback" (Tekrar Oynat) özelliği kullanılır. Konum `Limassol Marina` ve tarih/saat `26 Ekim 2024, 14:30` (UTC'ye çevrilerek) olarak ayarlanır.
    
-   **BULGU (ŞAŞIRTICI ANI):** `MarineTraffic` kaydı, o tarih ve saatte, devasa ve benzersiz (örn. yeşil gövdeli) **"MV Evergreen" konteyner gemisinin**, tam olarak "SecureData Solutions Ltd." şirketinin ofisinin bulunduğu rıhtımın önünden geçmekte olduğunu gösterir.
    
-   **Nihai Doğrulama (IMINT):** Analist, Adım 1'deki "belirsiz" fotoğrafa geri döner. Pencere yansımasındaki o "belirsiz lekenin", `MarineTraffic`'ten silüeti doğrulanan **"MV Evergreen" gemisinin gövdesi** ile mükemmel bir şekilde eşleştiğini fark eder.
    

**5\. Aşama: Finansal Analiz ve Görselleştirme (FININT)**

Artık kimliği ve konumu (hem dijital hem fiziksel olarak) doğrulanan hedefin finansal izleri incelenir:

-   **`Blockchair`** kullanılarak BTC cüzdanının işlem geçmişi incelenir. Paranın bir karıştırıcıya (mixer) gittiği, ancak cüzdana ilk test fonunun KYC (Müşterini Tanı) gerektiren `Coinbase` gibi bir borsadan geldiği görülür.
    
-   Bu karmaşık ilişki ağı (E-posta -> Sızıntı IP -> Şirket -> MARINT ile Doğrulanan Konum -> BTC Cüzdanı -> KYC'li Borsa), **`Maltego`** kullanılarak görselleştirilir. Bu, hedefin birden fazla kritik OpSec hatasını gösteren ve davayı sonuçlandıran somut bir analitik ürün (rapor) oluşturur.
    

___

### Bilgilendirme

Burada önerilen tüm kaynaklar, yöntemler ve araçlar bilgilendirme amaçlıdır. Bunları daha detaylı öğrenmek için kendi araştırmanızı yapınız. OSINT konusunda gelişmek istiyorsanız, alternatif senaryoları incelemeli, uygulamalı ve daha derin araştırmalar yapmalısınız.
