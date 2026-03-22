# 🖥️ Sentiric Web Agent

[![Status](https://img.shields.io/badge/status-prototype-orange.svg)]()
[![Framework](https://img.shields.io/badge/framework-Next.js_14-black.svg)](https://nextjs.org/)
[![Styling](https://img.shields.io/badge/styling-Tailwind_CSS_&_Tremor-blue.svg)]()

**Sentiric Web Agent UI**, insan müşteri hizmetleri temsilcileri (agent'lar) için tasarlanmış, tarayıcı tabanlı, modern bir çalışma alanıdır. Agent'ların çağrıları yönetmesini, müşteri bilgilerini anlık olarak görmesini ve AI ile işbirliği içinde çalışmasını sağlar.

## 🎯 Temel Sorumluluklar

*   **Çağrı Yönetimi:** Gelen çağrıları bir kuyrukta gösterir, agent'ların çağrıları kabul etmesini, devralmasını, sonlandırmasını, sessize almasını ve aktarmasını sağlar.
*   **Canlı Transkripsiyon:** Aktif bir görüşmenin canlı dökümünü (transkriptini) gerçek zamanlı olarak gösterir.
*   **Müşteri Bilgi Paneli (360° View):** Arayan müşterinin kim olduğunu, geçmiş etkileşimlerini ve CRM'den gelen diğer önemli bilgilerini tek bir ekranda sunar.
*   **AI İşbirliği:**
    *   **İzleme:** AI'ın müşteriyle yaptığı görüşmeyi sessizce dinleme.
    *   **Fısıldama (Whisper):** AI'a, müşterinin duymayacağı şekilde talimatlar veya ipuçları verme.
    *   **Devralma (Takeover):** Gerektiğinde tek bir tıklama ile görüşmenin kontrolünü AI'dan devralma.

## 🛠️ Teknoloji Yığını

*   **Framework:** Next.js 14
*   **Dil:** TypeScript
*   **Styling:** Tailwind CSS
*   **UI Bileşenleri:** Tremor (Veri görselleştirme için), Headless UI
*   **State Management:** Zustand
*   **Gerçek Zamanlı İletişim:** WebSocket (gelecekte)

## 🔌 API Etkileşimleri

Bu arayüz, platformla **sadece** `sentiric-api-gateway-service` üzerinden konuşur.

*   **Giden (İstemci):**
    *   `sentiric-api-gateway-service` (REST/JSON ve WebSocket): Tüm veri ve yönetim isteklerini bu merkezi kapıya yapar.

## 🚀 Yerel Geliştirme

1.  **Bağımlılıkları Yükleyin:** `npm install`
2.  **Geliştirme Sunucusunu Başlatın:** `npm run dev`
3.  Tarayıcınızda `http://localhost:3001` adresini açın.

## 🤝 Katkıda Bulunma

Katkılarınızı bekliyoruz! Lütfen projenin ana [Sentiric Governance](https://github.com/sentiric/sentiric-governance) reposundaki kodlama standartlarına ve katkıda bulunma rehberine göz atın.
---
## 🏛️ Anayasal Konum

Bu servis, [Sentiric Anayasası'nın (v11.0)](https://github.com/sentiric/sentiric-governance/blob/main/docs/blueprint/Architecture-Overview.md) **Zeka & Orkestrasyon Katmanı**'nda yer alan merkezi bir bileşendir.