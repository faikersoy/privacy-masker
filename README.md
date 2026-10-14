# 🛡️ Instant Offline AI Privacy Masker
### Anlık Çevrimdışı Yapay Zeka Gizlilik Maskeleyici

A lightweight, 100% client-side, single-file HTML/JS tool designed to automatically detect and mask Personally Identifiable Information (PII) before sending prompts or text data to Large Language Models (LLMs). 
> Büyük Dil Modellerine (LLM) prompt veya metin verisi göndermeden önce Kişisel Olarak Tanımlanabilir Bilgileri (PII) otomatik olarak tespit edip maskelemek için tasarlanmış, hafif, %100 istemci tarafında (tarayıcıda) çalışan tek dosyalık bir HTML/JS aracıdır.

Runs entirely within your browser's local memory with **zero external dependencies** and **zero data transit**, ensuring complete privacy and compliance with data governance standards (such as GDPR / KVKK).
> Hiçbir harici bağımlılık veya veri aktarımı olmaksızın tamamen tarayıcınızın yerel belleğinde çalışır; eksiksiz gizlilik ve veri yönetimi standartlarına (KVKK / GDPR gibi) uyumluluk sağlar.

---

## ✨ Key Features
### Başlıca Özellikler

* **100% Offline & Local / %100 Çevrimdışı ve Yerel:** No servers, no APIs, and no cloud logging. Your text never leaves your device. *(Sunucu, API veya bulut kaydı yoktur. Metniniz cihazınızdan asla çıkmaz.)*
* **Automatic Entity Detection / Otomatik Varlık Tespiti:** Uses optimized pattern matching and tokenization to identify sensitive data instantly without requiring manual pre-definition. *(Manuel ön tanımlamaya gerek kalmadan hassas verileri anında belirlemek için optimize edilmiş desen eşleştirme ve tokenizasyon kullanır.)*
* **Smart Non-Overlapping Engine / Akıllı Çakışmasız Motor:** Built-in priority and tokenization pass prevents overlapping regex bugs (cleanly separating phone numbers, 11-digit IDs/TC Kimlik numbers, credit cards, and IP addresses). *(Yerleşik öncelik ve tokenizasyon geçişi, çakışan regex hatalarını önler; telefon numaralarını, 11 haneli T.C. Kimlik numaralarını, kredi kartlarını ve IP adreslerini temiz bir şekilde birbirinden ayırır.)*
* **Proper Noun Heuristic / Özel İsim Sezgisel Analizi:** Automatically detects capitalized names and locations while filtering out common stopwords. *(Yaygın durdurma kelimelerini (stopwords) filtrelerken büyük harfle başlayan isimleri ve yerleri otomatik olarak tespit eder.)*
* **Zero Installation / Sıfır Kurulum:** Delivered as a single `.html` file—just save it and open it in any modern web browser. *(Tek bir `.html` dosyası olarak sunulur; kaydedin ve herhangi bir modern web tarayıcısında açın.)*

---

## 🔍 What It Automatically Masks
### Otomatik Olarak Maskelenen Veriler

| Entity Type / Veri Türü | Masked Output Tag / Maskelenmiş Etiket | Example Pattern / Format / Örnek Desen |
| :--- | :--- | :--- |
| **Email Addresses / E-Posta** | `[MASKED_EMAIL]` | `user@domain.com` |
| **Credit Cards / Kredi Kartı** | `[MASKED_CREDIT_CARD]` | `4532-7182-9304-8172` |
| **National IDs / T.C. Kimlik / SSN** | `[MASKED_TC_OR_SSN]` | `12345678901` (Strict 11-digit blocks) |
| **Phone Numbers / Telefon** | `[MASKED_PHONE]` | `+1-555-839-2049`, `05321234567` |
| **IPv4 Addresses / IPv4 Adresi** | `[MASKED_IPV4]` | `192.168.1.100` |
| **Names & Places / İsim ve Yerler** | `[MASKED_NAME]` | Proper nouns and capitalized entities *(Özel isimler)* |

---

---

---

## 🚀 How to Use & Offline Installation
### Nasıl Kullanılır ve Çevrimdışı Kurulum

You can use this tool either directly online via GitHub Pages, or download it to run 100% offline on your local machine:
> Bu aracı ister doğrudan çevrimiçi olarak GitHub Pages üzerinden kullanabilir, ister yerel makinenizde %100 çevrimdışı çalıştırmak için indirebilirsiniz:

### 1. Online Usage (Live Demo) / Çevrimiçi Kullanım (Canlı Demo)
* Simply visit the live web application: **[Live Demo Link](https://faikersoy.github.io/privacy-masker/)**
* *Canlı web uygulamasını ziyaret edin:* **[Canlı Demo Linki](https://faikersoy.github.io/privacy-masker/)**

### 2. Offline / Local Usage (Download ZIP) / Çevrimdışı / Yerel Kullanım (ZIP İndir)
1. Go to the main GitHub repository page: [GitHub Repository](https://github.com/faikersoy/privacy-masker)
2. Click the green **`<> Code`** button in the top right and select **`Download ZIP`**.
3. Extract the ZIP file and double-click the **`index.html`** file to run it instantly in your browser, even without an internet connection.

> 1. Ana GitHub depo sayfasına gidin: [GitHub Deposu](https://github.com/faikersoy/privacy-masker)
> 2. Sağ üstteki yeşil **`<> Code`** butonuna tıklayın ve **`Download ZIP`** seçeneğini seçin.
> 3. ZIP dosyasını klasöre çıkartın ve internet bağlantınız olmasa bile tarayıcınızda anında çalıştırmak için **`index.html`** dosyasına çift tıklayın.

---

## 🛠️ Built With
### Kullanılan Teknolojiler

* **Vanilla JavaScript (ES6+)**
* **HTML5 & CSS3 (Custom responsive dark theme / Özel duyarlı koyu tema)**

---

## 📄 License
### Lisans

This project is open-source and available under the [MIT License](LICENSE). *(Bu proje açık kaynaklıdır ve [MIT Lisansı](LICENSE) altında sunulmuştur.)*
