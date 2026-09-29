# Halil Sarıtaş

**Elektronik Mühendisi · AI & Full-Stack Developer · TurkuazCode**

Yapay zekâyı gerçek iş süreçlerine taşıyan, uçtan uca ürün geliştiren bir mühendisim. Dil modellerini (LLM) veritabanı, ödeme, mesajlaşma kanalları ve mobil uygulamalarla birleştirip sahada çalışan sistemler kuruyorum: e-ticaret müşteri asistanları, belediye mobil uygulamaları, eğitim platformları, belge analiz sistemleri ve şifreli bulut depolama.

Yaklaşımım: **model yorumlar, kod doğrular.** Yapay zekâ çıktısını fiyat, stok, sipariş ve kişisel veri gibi kritik noktalarda deterministik kod ve veritabanı kontrollerinden geçiriyorum. Çok kiracılı (multi-tenant) mimari, KVKK uyumu ve veri güvenliği her projede baştan tasarımın parçası.

> **English summary —** Electronics engineer and AI & full-stack developer building production AI products under TurkuazCode. I integrate LLMs (Gemini, OpenAI-compatible and self-hosted models) with PostgreSQL/pgvector, RAG pipelines, computer vision (CLIP), speech-to-text, payments and messaging channels (Instagram, WhatsApp). Shipped work spans multi-tenant SaaS, municipal mobile apps (React Native/Expo + Django), an education platform (NestJS, Flutter), document-analysis RAG systems and an end-to-end encrypted storage platform. Strong focus on multi-tenant isolation, KVKK/GDPR-style privacy and verifiable AI output.

---

## Öne Çıkan Projeler

> Projelerin çoğu ticari ya da kurumlara ait olduğu için kaynak kodu gizlidir. Teknik detaylar ve demo için iletişime geçebilirsiniz.

### TurkuazChat — Yapay zekâ destekli e-ticaret müşteri asistanı
Instagram ve WhatsApp'tan satış yapan mağazalar için 7/24 çalışan, çok kiracılı SaaS. Müşteri mesajını dil modeli yorumlar; ürün, stok, fiyat ve sipariş bilgisi kod tarafından veritabanından doğrulanır.
- Instagram DM, yorum, hikâye yanıtı ve WhatsApp webhook entegrasyonu; yoruma otomatik yanıt ve DM'e yönlendirme
- Fotoğraftan ürün bulma (CLIP görüntü gömmeleri + pgvector), RAG ile mağaza bilgi tabanı
- Çok adımlı sipariş, iade ve değişim akışları; insan temsilciye devir; gerçek zamanlı panel (WebSocket)
- Sağlayıcıdan bağımsız LLM katmanı (Gemini, OpenAI uyumlu API'ler, kendi sunucusunda barındırılan modeller)
- **Teknoloji:** Python, FastAPI, SQLAlchemy 2 (async), PostgreSQL + pgvector, React 18, TypeScript, TanStack Query, Tailwind, Docker

### DersAlem — Dershane yönetimi ve yapay zekâ destekli öğrenme platformu
Öğretmen, öğrenci, veli ve yönetici rollerine sahip çok kiracılı B2B SaaS.
- Flutter mobil uygulama, React yönetim paneli, NestJS API
- Optik form okuma (OMR) servisi: Python, FastAPI, OpenCV
- **Teknoloji:** TypeScript monorepo (pnpm, Turborepo), NestJS, Prisma, PostgreSQL, Redis, MinIO, Flutter, Docker

### Ermenek ve Güneyyurt Belediyesi Mobil Uygulamaları
İki belediye için yayına hazır vatandaş hizmetleri uygulamaları: haberler, şikâyet/öneri (fotoğraflı), bilgi edinme, nöbetçi eczane, canlı kameralar, şehir rehberi.
- Yapay zekâ asistanı: belediye mevzuatı ve belgeleri üzerinde RAG; gömmeler (BGE-M3) kişisel veri dışarı çıkmadan kendi sunucuda hesaplanıyor
- KVKK onay ve veri silme akışları
- **Teknoloji:** React Native (Expo), Django REST Framework, PostgreSQL; ayrıca React + Express tabanlı kurumsal web sitesi

### YapıAI — Yapım işleri için belge analiz platformu
İnşaat ve yapım işleri belgelerini (PDF, DOCX, Excel, taranmış belgeler) analiz eden, soru-cevap yapan RAG sistemi.
- Yerel embedding (BGE-M3) ve HNSW vektör arama; OCR (Tesseract)
- Çoklu LLM desteği: Gemini, OpenRouter, LM Studio, Ollama; SearXNG ile web araması
- **Teknoloji:** Node.js, Express, MongoDB, React

### Adalet Bulut — Uçtan uca şifreli bulut depolama
Ekipler için güvenli dosya depolama ve paylaşım platformu.
- AES-256-GCM dosya şifreleme, Argon2id parola hash'leme, JWT, hız sınırlama, CSP
- Sürümleme, çöp kutusu, şifreli paylaşım bağlantıları, denetim kaydı, otomatik yedekleme
- **Teknoloji:** React, Node.js, PostgreSQL, Docker

### QR Menü — Restoranlar için dijital menü ve canlı sipariş
Çok kiracılı QR menü, masadan sipariş ve ödeme sistemi.
- Socket.io ile mutfak ve garsona canlı sipariş; rol bazlı yetki (yönetici, garson, mutfak)
- Kiracıya özel sanal POS entegrasyonu, POS anahtarları veritabanında AES-256-GCM ile şifreli; fiyatlar sunucuda hesaplanır
- **Teknoloji:** Next.js 16, TypeScript, Prisma 7, PostgreSQL, Auth.js v5, Tailwind v4, shadcn/ui

### Proje Takip — Yapım işleri ilerleme, hakediş ve fiyat farkı sistemi
Kamu yapım işlerinde proje ilerlemesi, hakedişler ve yıllık fiyat farkı hesaplarının takibi.
- **Teknoloji:** React 19, Node.js, PostgreSQL

### Anlarım — Etkinlikler için QR ile fotoğraf paylaşımı
Düğün ve organizasyonlarda misafirlerin uygulama indirmeden fotoğraf/video yüklediği platform; canlı duvar, yapay zekâ ile davetiye metni, iyzico ile paket satışı.
- **Teknoloji:** Next.js, PostgreSQL, Cloudflare R2, iyzico

---

## Teknik Yetkinlikler

| Alan | Teknolojiler |
|---|---|
| **Yapay zekâ / LLM** | RAG, embedding ve vektör arama (pgvector, ChromaDB, HNSW), araç çağırma ve niyet yönlendirme, yapılandırılmış çıktı doğrulama, CLIP ile görsel arama, faster-whisper ile konuşmadan metne, OCR, Gemini, OpenAI uyumlu API'ler, Ollama / LM Studio ile yerel model barındırma |
| **Backend** | Python (FastAPI, Flask, Django), Node.js (Express, NestJS), Celery, Redis, WebSocket / Socket.io, REST API tasarımı |
| **Frontend** | React, Next.js, TypeScript, Tailwind CSS, shadcn/ui, TanStack Query, Zustand, Vite |
| **Mobil** | React Native (Expo), Flutter |
| **Veri** | PostgreSQL, pgvector, Prisma, SQLAlchemy, Alembic, MongoDB |
| **Altyapı** | Docker, Docker Compose, Linux VPS, Vercel, Railway, Cloudflare R2, GitHub Actions |
| **Güvenlik ve uyum** | Çok kiracılı veri izolasyonu, KVKK, AES-256-GCM, Argon2id, JWT + httpOnly refresh token, webhook imza doğrulama, hız sınırlama |
| **Entegrasyonlar** | Instagram Graph API, WhatsApp (Cloud API, WAHA), iyzico, sanal POS, ikas |

## Eğitim

- **Elektronik ve Haberleşme Mühendisliği** — Süleyman Demirel Üniversitesi (2014–2018)
- İngilizce Hazırlık — Süleyman Demirel Üniversitesi (2013–2014)

## Sertifikalar

| Sertifika | Kurum | Tarih |
|---|---|---|
| React JS v18 | BTK Akademi | Ocak 2025 |
| Node.js ile Web Programlama | BTK Akademi | Şubat 2025 |
| Scrum | BTK Akademi | Şubat 2025 |
| Problem Çözme Teknikleri | BTK Akademi | Şubat 2025 |
| HTML5 ile Web Geliştirme | BTK Akademi | Aralık 2024 |
| Microsoft Excel Temelleri | BTK Akademi | Kasım 2024 |
| Yazılım geliştirme sertifika programları | Boğaziçi Enstitüsü | 2024 |

## Açık Kaynak Referans Arşivi

Aşağıdaki depolar, çalışmalarımda başvurduğum açık kaynak yapay zekâ projelerinin **salt okunur arşiv kopyalarıdır**; benim eserim değildir. Tüm hakları orijinal geliştiricilerine aittir ve her biri kendi lisansıyla dağıtılır (açıklamalarında kaynak ve lisans belirtilmiştir).

- **Yerel LLM çalıştırma:** llama.cpp, ollama, vllm
- **Arayüz ve ajan:** open-webui, dify, langchain, langgraph
- **Ses ve görüntü:** whisper, faster-whisper, ComfyUI, open_clip
- **Eğitim ve öğrenme:** nanoGPT, llm.c, minbpe, transformers; ayrıca Türkçe açıklamalı minGPT çalışmam
- **Açık ağırlıklı modeller:** Qwen3.8, GLM-5, Kimi-K3, DeepSeek-V3

## İletişim

- E-posta: turkuazcode@gmail.com
- LinkedIn: [linkedin.com/in/halil-sarıtaş-062b0a166](https://www.linkedin.com/in/halil-sar%C4%B1ta%C5%9F-062b0a166/)
- GitHub: [github.com/hsrts](https://github.com/hsrts)

<details>
<summary>Profil özeti (makine tarafından okunabilir)</summary>

```yaml
name: Halil Sarıtaş
title: Electronics Engineer · AI & Full-Stack Developer
organization: TurkuazCode
location: Türkiye
languages: [Turkish (native), English]
education:
  - degree: B.Sc. Electronics and Communication Engineering
    school: Süleyman Demirel University
    years: 2014-2018
focus_areas:
  - Production LLM applications (RAG, tool routing, output verification)
  - Multi-tenant SaaS architecture
  - Conversational commerce (Instagram, WhatsApp)
  - Municipal and public-sector mobile apps
  - Privacy by design (KVKK), encryption
primary_stack:
  ai: [Gemini, OpenAI-compatible APIs, self-hosted LLMs, pgvector, ChromaDB, CLIP, faster-whisper, BGE-M3]
  backend: [Python, FastAPI, Flask, Django, Node.js, Express, NestJS, Celery, Redis]
  frontend: [React, Next.js, TypeScript, Tailwind CSS]
  mobile: [React Native, Expo, Flutter]
  data: [PostgreSQL, Prisma, SQLAlchemy, MongoDB]
  infra: [Docker, Linux VPS, Vercel, Railway]
products:
  - {name: TurkuazChat, type: AI customer assistant SaaS for e-commerce, stack: [FastAPI, PostgreSQL, pgvector, React]}
  - {name: DersAlem, type: Education management & AI learning SaaS, stack: [NestJS, Prisma, Flutter, React, OpenCV]}
  - {name: Ermenek & Güneyyurt Municipality apps, type: Citizen services mobile apps with RAG assistant, stack: [React Native, Expo, Django]}
  - {name: YapıAI, type: Construction document analysis RAG platform, stack: [Node.js, MongoDB, React, BGE-M3]}
  - {name: Adalet Bulut, type: End-to-end encrypted cloud storage, stack: [React, Node.js, PostgreSQL]}
  - {name: QR Menü, type: Multi-tenant QR menu, live ordering and payments, stack: [Next.js, Prisma, Socket.io]}
  - {name: Proje Takip, type: Construction progress, progress payment and price escalation tracking, stack: [React, Node.js, PostgreSQL]}
  - {name: Anlarım, type: Event photo sharing via QR, stack: [Next.js, PostgreSQL, Cloudflare R2, iyzico]}
contact:
  email: halilsrts70@gmail.com
  linkedin: https://www.linkedin.com/in/halil-sar%C4%B1ta%C5%9F-062b0a166/
```

</details>
