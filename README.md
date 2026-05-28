# Kardelen JIT Optimization BaaS

Kardelen, yapay zeka destekli, otonom darboğaz çözen bir **AOT (Ahead-of-Time) / JIT (Just-in-Time) derleyici** hizmetidir. Ağır hesaplama gerektiren döngüleri çalışma zamanında tespit eder, Gemini API aracılığıyla matematiksel eşdeğerlerine ($O(1)$ karmaşıklığına) dönüştürür ve sistem performansını maksimize eder.

---

## 🚀 Temel Özellikler

*   **Melez Derleyici (Hybrid Compiler):** Kaynak kodun sözcüksel ve sözdizimsel analizini yaparak gelişmiş AST yönetimi sağlar.
*   **AI Destekli Darboğaz Çözücü:** Profiling tabanlı Gemini API entegrasyonu ile darboğazları tespit eder ve optimize eder.
*   **AOT Önbellek (Cache) Sistemi:** Optimize edilmiş algoritmaları JSON tabanlı kalıcı depoda saklayarak tekrarlanan işlemleri hızlandırır.
*   **Hot-Swap Sanal Makine:** Güvenli OSR (On-Stack Replacement) mekanizması ile çalışma zamanında kod değişimi ve otomatik rollback sağlar.
*   **BaaS API:** FastAPI tabanlı, ölçeklenebilir ve otonom optimizasyon uç noktaları sunar.

---

## 🛠️ Yol Haritası (Geliştirilecek Özellikler)

### Güvenlik ve İzolasyon
*   **Sandbox Yürütme:** gVisor veya Docker cgroups ile izole edilmiş güvenli kod çalıştırma ortamı.
*   **Kod İmzalama:** API düzeyinde istek doğrulama ve kod bütünlüğü imzalama mekanizması.

### Optimizasyon ve Doğrulama
*   **Formal Doğrulama:** Orijinal kod ve optimize edilmiş kod arası sonuç tutarlılığı testi.
*   **Optimizasyon Güven Skoru:** Belirli eşiklerin üzerindeki AI çıktılarının otomatik uygulanması.

### Ölçeklenebilirlik
*   **Event-Driven Mimari:** Webhook ve `job_id` tabanlı asenkron durum sorgulama.
*   **Dağıtık Kuyruk:** Celery/Redis ile optimizasyon süreçlerinin ana akıştan ayrıştırılması.

### Geliştirici Deneyimi (DX)
*   **Stack Trace Mapping:** Hata durumunda orijinal kaynak koda yönlendiren *source-map* yapısı.
*   **Visualizer/Diff:** Kullanıcıya özel kod değişim görselleştirme arayüzü.

### AI Modeli Esnekliği
*   **Model Gateway:** Llama 3, Claude veya özel SLM modelleri için model bağımsız mimari.

---

## 🏗️ Teknoloji Yığını
*   **Core:** Python 3.11, AST, Lexical Analysis.
*   **AI:** Google GenAI SDK (Gemini 2.5-Flash).
*   **API:** FastAPI, Uvicorn, Pydantic.
*   **Containerization:** Docker, Build-essential.

---

## Görseller 
<img width="1328" height="742" alt="image" src="https://github.com/user-attachments/assets/18f4526d-8e74-41d6-9d93-11b705aeb622" />
<img width="1322" height="742" alt="image" src="https://github.com/user-attachments/assets/456443ce-b2d7-4c8d-add9-94c3c6f0ff5f" />
<img width="1325" height="723" alt="image" src="https://github.com/user-attachments/assets/b50e92d4-f5d3-4be8-9c31-f6f71afda9e7" />
<img width="1323" height="733" alt="image" src="https://github.com/user-attachments/assets/5e75939e-5543-4714-b622-d2bdf690ffb0" />
<img width="1322" height="711" alt="image" src="https://github.com/user-attachments/assets/9c5282fd-3173-49c9-9f15-72fc8b9ecb7a" />
<img width="1321" height="744" alt="image" src="https://github.com/user-attachments/assets/e05828ab-6e8c-4049-9c33-d5b62b57a2cb" />
<img width="1326" height="726" alt="image" src="https://github.com/user-attachments/assets/f6deb322-d6a9-4d6e-a21d-059e838dfab9" />
<img width="1327" height="716" alt="image" src="https://github.com/user-attachments/assets/df876dd8-adfb-4698-9d4a-c81f20eecf14" />
<img width="1326" height="717" alt="image" src="https://github.com/user-attachments/assets/36cef69d-f31d-40eb-88ef-f0e88dac988b" />
<img width="1326" height="723" alt="image" src="https://github.com/user-attachments/assets/34f9147c-b01b-4204-84e3-7c56a5242895" />
<img width="1325" height="706" alt="image" src="https://github.com/user-attachments/assets/08edbd43-a9d7-4708-8ba1-d5422309d137" />


*Kardelen Projesi | Teknik Dökümantasyon v7.2 | 2026*
