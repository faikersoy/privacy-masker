# 🛡️ Instant Offline AI Privacy Masker

A lightweight, 100% client-side tool designed to automatically detect and mask Personally Identifiable Information (PII) before sending prompts or text data to Large Language Models (LLMs). Runs entirely within your browser's local memory with zero external dependencies.

Büyük Dil Modellerine (LLM) veri göndermeden önce kişisel bilgileri otomatik olarak maskeleyen %100 yerel ve çevrimdışı araçtır. Verileriniz tarayıcınızdan asla çıkmaz.

---

## ✨ Features / Özellikler

* **🔒 100% Client-Side & Privacy-First:** No server-side processing, no data logging, and zero external network requests (even the favicon is embedded locally).
* **⚡ Real-Time Masking:** Instant sanitization as you type or paste text into the input field (`oninput` optimized).
* **🇹🇷 Turkish Suffix Support:** Smartly handles Turkish proper nouns with apostrophes (e.g., `ankara'da`, `İstanbul'dan` -> `[MASKED_NAME]'da`).
* **🔢 Unified Sensitive Number Masking:** Consolidates phone numbers, national IDs, and general numeric identifiers under a clean **`[MASKED_NO]`** tag.
* **🌐 Strict IP & Format Validation:** Validates IPv4 octets (0–255) to prevent false positives while accurately masking valid IPs, emails, and credit cards.
* **🚫 Stopword & Sentence-Start Filtering:** Prevents ordinary sentence-starting words from being mistakenly flagged as proper nouns.

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
👉 **[https://faikersoy.github.io/privacy-masker/](https://faikersoy.github.io/privacy-masker/)**

---

## 💻 Tech Stack / Kullanılan Teknolojiler

* **HTML5 / Vanilla JavaScript (ES6+)**
* **CSS3 (Modern Custom Properties & Responsive Flexbox/Grid)**
* **Embedded SVG Data URI (Zero external asset dependencies)**

---

## 📜 License / Lisans

This project is open-source and available under the [MIT License](LICENSE).
