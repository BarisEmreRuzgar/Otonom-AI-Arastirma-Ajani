<div align="center">
  
# 🤖 Otonom ArXiv Yapay Zeka Araştırma Ajanı

[![n8n](https://img.shields.io/badge/n8n-Workflow_Automation-FF6666?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT_4o--mini_&_TTS-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Telegram](https://img.shields.io/badge/Telegram-Bot_API-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://core.telegram.org/bots)
[![Google Sheets](https://img.shields.io/badge/Google_Sheets-Database-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)](https://workspace.google.com/products/sheets/)

**ArXiv üzerinden yapay zeka makalelerini analiz eden, puanlayan ve raporlayan uçtan uca otonom sistem.**

</div>

---

## 📢 Proje Hakkında

Bu proje, ArXiv (cs.AI) üzerinden bilgisayar bilimleri ve yapay zeka makalelerini otonom olarak takip eden, büyük dil modelleri (LLM) ile analiz edip filtreleyen ve sonuçları çoklu kanaldan (ses, metin, veritabanı) raporlayan uçtan uca bir n8n iş akışıdır. Sistem, bilgi kirliliğini önlemek amacıyla yalnızca yüksek kaliteli akademik araştırmaları kullanıcıya ulaştırmak üzere tasarlanmıştır.

---

## ✨ Teknik Özellikler

| Özellik | Açıklama |
| :--- | :--- |
| 📡 **Akıllı Veri Çekme** | ArXiv RSS feed (cs.AI) üzerinden en güncel akademik makaleleri otomatik toplar. |
| 🧠 **LLM Tabanlı Puanlama** | OpenAI modelleri ile makalelerin yenilikçiliğini analiz eder, 1-10 arası skorlar ve 3 maddelik özet çıkarır. |
| 🛡️ **Otonom Filtreleme** | Sadece 7 ve üzeri puan alan vizyoner ve kaliteli makaleleri akıştan geçirir. |
| 🎙️ **Sesli Brifing (TTS)** | Filtreyi geçen makale özetlerini Text-to-Speech (nova) ile sesli formata (.mp3) dönüştürür. |
| 📱 **Çoklu Kanal Dağıtımı** | Analiz sonuçlarını, ses dosyasını ve linki Telegram botu üzerinden doğrudan iletir. |
| 🗄️ **Kalıcı Arşivleme** | Makale başlığı, skoru, özeti ve linkini otonom olarak Google Sheets veritabanına kaydeder. |

---

## 🛠️ Kullanılan Teknolojiler

*   **n8n:** Node tabanlı görsel iş akışı otomasyonu.
*   **OpenAI API:** Yapay zeka hakemliği (puanlama), çeviri, özetleme (Structured Outputs) ve ses sentezi (TTS).
*   **Telegram Bot API:** Kullanıcı arayüzü, Inline klavye butonları ve sesli mesaj iletimi.
*   **Google Workspace API:** Yapay zeka araştırma kütüphanesi için otonom tablo yönetimi.

---

## 🚀 Kurulum ve Kullanım

1.  **n8n Kurulumu:** Yerel veya bulut (n8n Cloud) tabanlı bir n8n örneği başlatın.
2.  **Akışı İçe Aktarma:** Bu depodaki `.json` uzantılı dosyayı indirip n8n ekranında **"Import from File"** seçeneği ile yükleyin.
3.  **Kimlik Bilgileri (Credentials):**
    *   OpenAI API anahtarınızı LLM ve TTS düğümlerine ekleyin.
    *   Telegram Bot Token'ınızı ekleyin.
    *   Google Sheets düğümüne Google Workspace OAuth yetkisi verin.
4.  **Başlatma:** Akışı "Active" (Yayınla) konumuna getirin. Sistem belirlediğiniz zamanlamada (örneğin hafta içi her gün 09:00) otonom olarak çalışacaktır.

---

<div align="center">

**Geliştirici**

**Barış Emre Rüzgar**

[![GitHub](https://img.shields.io/badge/GITHUB-BARISEMRERUZGAR-black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/BarisEmreRuzgar)


</div>
