<p align="center">
  <picture>
    <source media="(max-width: 900px)" srcset="https://github.com/ceceys/ceceys/raw/main/cecey-mobile.gif">
    <img src="cecey.gif" alt="cecey terminal" width="100%">
  </picture>
</p>

# Cuma Ali Dirik (cecey)

İstanbul'da yazılım ve BT alanında çalışıyorum. İşte karşılaştığım sorunlar için araçlar yazmayı seviyorum, bir kısmını da açık kaynak olarak paylaşıyorum. Aşağıda bunlarla birlikte üzerinde çalıştığım bazı işler var.

[English](README.md)

## Nasıl çalışırım

- **Kaynağa dokunmam.** Araçlarım veriyi kopyalar ya da okur, aslını değiştirmez.
- **Her adım geri alınabilir.** Taşıma ve düzenlemeleri kayıt altında tutarım, gerektiğinde geri dönülebilir.
- **Doğrulamadan bitti demem.** Sayıları karşılaştırır, dosyaları SHA-256 ile denetler, çıktıyı gerçek örneklerle test ederim.
- **Veri kullanıcıda kalır.** Telemetri koymam, güncellemeler sormadan kurulmaz.

## Açık kaynak

| Proje | Ne işe yarar | Teknoloji |
|---|---|---|
| [Mandal](https://github.com/ceceys/mandal) | Windows'ta ekran alıntıları ve notlar için çamaşır ipi: alıntı al, ipe as, kopyala, görseli metne çevir, kartlara kısayol ata. | C#, WPF, .NET 8, Windows OCR, Inno Setup, GitHub Actions |
| [SWIFT PDF](https://github.com/ceceys/swift-pdf) | Kuveyt Türk giden transfer mailinden yalnız ham SWIFT metnini içeren tek sayfa A4 PDF üretir.<br>**Etki:** Elle yapılan iş birkaç saniyeye indi; 298 test PDF'inin 298'inde doğru. | C#, WPF, .NET 8, PdfPig, WebView2 |
| [Mail Aktarıcı](https://github.com/ceceys/mail-aktarici) | Outlook hesaplarını, PST arşivlerini ve IMAP/POP3 kutularını kaynağa dokunmadan tek klasöre kopyalar, sayıları doğrular. | C#, WinForms, .NET Framework 4, Outlook COM |
| [Dijital Gözetleme Kulesi](https://github.com/ceceys/dijital-gozetleme-kulesi) | WatchTower: sitelerin erişimini, HTTP durumunu, SSL ve alan adı bitişini her gün denetler.<br>**Etki:** Her gün elle yapılan site kontrolü otomatikleşti. | VB.NET, WHOIS |

## Kurum içi yazılımlar

| Proje | Ne işe yarar | Teknoloji |
|---|---|---|
| Yardım masası | Bilet, zimmet formu ve gün sonu raporlamasını tek yerde toplar.<br>**Etki:** Her gün kullanılıyor; performans düzeltmesiyle %90 hızlandı. | PHP 8, MariaDB, Tailwind CSS, Chart.js, Gemini API |
| Müşteri ekstre gönderici | Hesap ekstrelerini tek ekrandan önizleyip onaylayarak hazırlar ve gönderir.<br>**Etki:** Elle yapılan bir işin yerini aldı. | PHP, MariaDB |
| Bülten ve toplu mail | Kişiselleştirilmiş, abonelikten çıkma bağlantılı ve hız sınırlı bülten gönderir.<br>**Etki:** Yılda 30-50 bin TL'lik mailing masrafı kalktı. | PHP, cron, SPF / DKIM / DMARC |
| Haber ve blog botu | Seçilen kaynakları tarar, site için görselli özgün yazı taslakları hazırlar.<br>**Etki:** Aylık ~75 $'lık bir hizmetin işini sıfır maliyetle yapıyor. | PHP, Gemini API |
| PDF çeviri aracı | Yabancı dildeki PDF'leri sayfa düzenini koruyup çeviriyi üstüne bindirerek Türkçeye çevirir.<br>**Etki:** Sayfa sınırı yok, aynı gün; dışarıdan çeviri hizmeti ihtiyacı kalktı. | PHP, Python, Gemini API |
| Ofis sohbet | Görsel ve GIF paylaşımlı, tek odalı ekip sohbeti. | PHP, MariaDB, JavaScript |
| Kaza tazminat hesaplayıcı (geliştiriliyor) | Trafik kazası dosyalarında mahrumiyet bedeli, değer kaybı ve hasar hesabı yapar, bilirkişi raporu biçiminde PDF üretir ve emsal karar bulur. | PHP 8.2, MariaDB, mPDF, PhpSpreadsheet, Gemini API, Tailwind |

## Otomasyon

| Proje | Ne işe yarar | Teknoloji |
|---|---|---|
| Muhasebe arşivi düzenleyici | Muhasebe dosyalarını içeriğine bakarak (OCR dahil) düzenler ve her taşımayı geri alınabilir tutar.<br>**Etki:** 32.368 dosya düzenlendi; SHA-256 ile tek belgenin kaybolmadığı doğrulandı. | Python, Tesseract OCR, SQLite, PowerShell |
| Sosyal medya üretim hattı | Kaynak belgeden gönderi, story, Reels ve X dizisi üretir, kaynakta olmayan rakamı eler, onaya sunar ve onaylananı zamanında yayınlar.<br>**Etki:** Bir markanın gönderi stoğu 0,1 günden 1,8 güne çıktı. | Python, PHP, Meta API'leri, Claude |
| Search Console aracı | Alan adlarını Google Search Console'a ekler, DNS üzerinden doğrular, site haritası gönderir ve tıklama verisini çeker.<br>**Etki:** Site haritası ve doğrulama siteler genelinde otomatikleşti. | Python, Search Console API, Cloudflare API |
| Alan adı bitiş takvimi | Bitiş tarihlerini whois ve RDAP'tan okuyup tarih sıralı tablo yapar.<br>**Etki:** Yönetilen tüm alan adlarının bitiş tarihi tek yerden izleniyor. | Python, whois, RDAP |
| Outlook posta kutusu düzeni | Klasik Outlook için sıralama kuralları ve yıllara göre arşiv.<br>**Etki:** Gelen kutusu 6.110 iletiden 37'ye indi. | Outlook COM otomasyonu |

## Web siteleri

Sıfırdan yazılan ya da baştan yapılan siteler, çoğu kendi yönetim paneliyle.

| Site | Ne | Teknoloji |
|---|---|---|
| Şirket sitesi | Yönetim paneli ve içerik baştan yapıldı, SEO yenilendi.<br>**Etki:** 87 sayfa yeniden yazıldı. | PHP, Tailwind |
| Çok dilli kurumsal site | Türkçe girilen içerik üç dile kendiliğinden çevriliyor. | PHP, MySQL, Gemini |
| Blog platformu | Yazıların yönetim panelinden yayınlandığı platform; yeni sürümü yapılıyor. | PHP, MySQL, Tailwind |
| İki dilli ürün kataloğu | Sektör, ürün ve proje sayfaları veritabanından geliyor. | PHP, MySQL |
| Restoran sitesi | Eski WordPress sitesinin yerine sıfırdan yazıldı.<br>**Etki:** Yıllık işletme gideri %60 azaldı. | PHP, MySQL |
| Küçük işletme siteleri | İmalat ve atölye işletmeleri için fotoğraf yüklemeli teklif formları, yönetim panelleri ve yapılandırılmış veri.<br>**Etki:** Bir site 324 MB'tan 28 MB'a indi; yavaş 4G'de LCP 1,9 sn. | PHP, MariaDB, Python, Playwright, JSON-LD |
| Servis yönetim uygulaması | Bir tamir dükkânı için servis kabul, satış ve stok, müşteri bildirimleriyle. | PHP, MariaDB, Tailwind |
| Restoran adisyon sistemi | Mutfak ekranı, masa, menü, stok, QR menü ve fiş yazıcısı. | PHP, MySQL, Tailwind, Chart.js, ESC/POS |

<details>
<summary><b>Denemeler ve eski projeler</b></summary>

| Proje | Ne işe yarar | Teknoloji |
|---|---|---|
| Domiva | Köy, ordu, klan ve savaş katmanlı, çok oyunculu tarayıcı strateji oyunu. | PHP, MySQL, JavaScript |
| Stajyer eğitim oyunu | Stajyerlere bulmaca olarak gönderilen, Windows 95 temalı altı bölümlü dedektiflik oyunu. | — |
| Nexus | İşi yönetici, ağ, sistem ve analist ajanlarına bölen çok ajanlı "sanal BT departmanı". | Python, CrewAI, FastAPI, ChromaDB |
| İşlem sinyali çalışması | Kural tabanlı demo işlem botu ve bir Telegram sinyal kanalını ölçen dinleyici; plasebo testinde rastgele girişler kanalın sinyallerini geçti. | Python, MetaTrader 5, SQLite |
| Satın alma programı | Tedarikçiden teklif toplar, fiyat karşılaştırır, sipariş ve teslimatı izler. | C# WinForms, sonra PHP |

</details>

<details>
<summary><b>Küçük araçlar</b></summary>

- Sesi yerelde Türkçe metne çeviren döküm aracı (Python, faster-whisper)
- Ekran görüntülü ve SHA-256'lı marka ihlali delil toplayıcı (Python)
- Instagram arşivleyici ve Reels üretici (Python, Meta Graph API)
- Google öneri motorundan anahtar kelime toplayıcı (Python)
- Cloudflare Workers ile site haritası sunumu (JavaScript)
- Geri alınabilir klasör düzenleme betikleri (Python)
- Tatil takvimi ve döviz kuru şeridi bileşenleri (HTML, JavaScript)

</details>

<details>
<summary><b>Meraklısı için tüm yetkinliklerim</b></summary>

| Alan | Yetkinlikler |
|---|---|
| **Yazılım geliştirme** | **Diller:** Python (ileri seviye), C, C++, C#, Java, Go, Rust, Kotlin, Dart, PHP, VB.NET, JavaScript, TypeScript, MQL5<br>**Masaüstü:** .NET, WPF, XAML<br>**Web:** React, Vue, Next.js, Laravel, Node.js, FastAPI<br>**Veritabanı:** MySQL, MSSQL, NoSQL<br>**Betik:** PowerShell, Bash, Batch, VBA, Lua<br>**Araçlar:** Git, GitHub, Docker |
| **Sistem ve altyapı** | **Sunucu:** Windows Server, IIS, Active Directory<br>**Linux:** Debian, Ubuntu, Arch Linux<br>**Sanallaştırma:** Proxmox, VMware, Hyper-V, VirtualBox<br>**Barındırma:** Nginx, Apache, Plesk, cPanel<br>**E-posta:** Kendi sunucusunda çalışan e-posta sistemleri, yedekleme ve iş sürekliliği<br>**Donanım:** Sunucu, istemci ve ağ kurulumu, arıza tespiti, onarım |
| **Ağ ve siber güvenlik** | **Güvenlik:** Güvenlik duvarı ve yönlendirici yönetimi, VPN, erişim denetimi<br>**Analiz:** Wireshark, Nmap, Kali Linux, kayıt analizi<br>**Koruma:** Fidye yazılımına karşı yedekleme stratejileri<br>**Kenar:** Cloudflare ile DNS ve uygulama güvenliği |
| **Otomasyon ve yapay zekâ** | **Otomasyon:** Python, PowerShell, n8n, raporlama ve izleme<br>**Yapay zekâ:** LLM API, CrewAI, Ollama, Whisper, Hugging Face, OCR |
| **Tasarım ve dijital pazarlama** | **Tasarım:** Photoshop, Illustrator, Figma, Canva, Blender, Premiere, After Effects<br>**Pazarlama:** Google Ads, Analytics, Meta Business Suite, Search Console, SEO |

</details>
