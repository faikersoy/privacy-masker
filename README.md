# 🛡️ Instant Offline AI Privacy Masker

A lightweight, 100% client-side tool designed to automatically detect and mask Personally Identifiable Information (PII) before sending prompts or text data to Large Language Models (LLMs). Runs entirely within your browser's local memory with zero external dependencies.

*Büyük Dil Modellerine (LLM) veri göndermeden önce kişisel bilgileri otomatik olarak maskeleyen %100 yerel ve çevrimdışı araçtır. Verileriniz tarayıcınızdan asla çıkmaz.*

---

## ✨ Features / Özellikler

* **🔒 100% Client-Side & Privacy-First / %100 İstemci Taraflı ve Gizlilik Odaklı:** No server-side processing, no data logging, and zero external network requests (even the favicon is embedded locally). / *Sunucu tarafında işlem yapılmaz, veri günlüğü tutulmaz ve sıfır harici ağ isteği gerçekleşir (favicon bile yerel olarak gömülüdür).*
* **⚡ Real-Time Masking / Anlık Canlı Maskeleme:** Instant sanitization as you type or paste text into the input field (`oninput` optimized). / *Girdi alanına metin yazdığınız veya yapıştırdığınız anda anında temizleme sağlar (`oninput` ile optimize edilmiştir).*
* **🇹🇷 Turkish Suffix Support / Türkçe Ek Desteği:** Smartly handles Turkish proper nouns with apostrophes (e.g., `ankara'da`, `İstanbul'dan` -> `[MASKED_NAME]'da`). / *Kesme işareti içeren Türkçe özel isim eklerini akıllıca yönetir (örn. `ankara'da`, `İstanbul'dan` -> `[MASKED_NAME]'da`).*
* **🔢 Unified Sensitive Number Masking / Birleştirilmiş Hassas Numara Maskeleme:** Consolidates phone numbers, national IDs, and general numeric identifiers under a clean **`[MASKED_NO]`** tag. / *Telefon numaralarını, TC kimlik numaralarını ve genel sayısal tanımlayıcıları temiz bir **`[MASKED_NO]`** etiketi altında toplar.*
* **🌐 Strict IP & Format Validation / Sıkı IP ve Format Doğrulaması:** Validates IPv4 octets (0–255) to prevent false positives while accurately masking valid IPs, emails, and credit cards. / *Geçerli IP'leri, e-postaları ve kredi kartlarını doğru bir şekilde maskelerken yanlış pozitifleri önlemek için IPv4 oktetlerini (0–255) doğrular.*
* **🚫 Stopword & Sentence-Start Filtering / Durak Kelime ve Cümle Başı Filtreleme:** Prevents ordinary sentence-starting words from being mistakenly flagged as proper nouns. / *Sıradan cümle başı kelimelerin yanlışlıkla özel isim olarak işaretlenmesini engeller.*

---

## 🏷️ Supported Tags / Desteklenen Etiketler

| Entity Type / Varlık Türü | Mask Tag / Maske Etiketi | Example / Örnek |
| :--- | :--- | :--- |
| **Proper Nouns / Yer & İsimler** | `[MASKED_NAME]` | Ahmet Yılmaz, ankara'da $\rightarrow$ `[MASKED_NAME]'da` |
| **Phones & IDs / Telefon & Kimlik** | `[MASKED_NO]` | +90 532 123 45 67, 12345678901 |
| **Email Addresses / E-postalar** | `[MASKED_EMAIL]` | ahmet.yilmaz@sirket.com |
| **Credit Cards / Kredi Kartları** | `[MASKED_CREDIT_CARD]` | 4532 7812 3456 7890 |
| **IPv4 Addresses / IP Adresleri** | `[MASKED_IPV4]` | 192.168.1.50 |

---

## 🚀 Live Demo / Canlı Demo

Access the live application hosted on GitHub Pages:  
*GitHub Pages üzerinde yayınlanan canlı uygulamaya erişin:*  
👉 **[https://faikersoy.github.io/privacy-masker/](https://faikersoy.github.io/privacy-masker/)**

---

## 💻 Tech Stack / Kullanılan Teknolojiler

* **HTML5 / Vanilla JavaScript (ES6+)**
* **CSS3 (Modern Custom Properties & Responsive Flexbox/Grid)**
* **Embedded SVG Data URI (Zero external asset dependencies / Sıfır harici varlık bağımlılığı)**

---

## 📜 License / Lisans

This project is open-source and available under the [MIT License](LICENSE).  
*Bu proje açık kaynaklıdır ve [MIT Lisansı](LICENSE) altında sunulmuştur.*
