# Paintly Paint — Oturum Özeti (1–5 Kasım 2026)

**Depo (kod, özel):** `UfukAntep/paintly-paint-source` · çalışma dalı `claude/wonderful-mayer-79udp5`, her şey `main`'e de gönderildi (son commit `055797f`).
**Herkese açık depo:** `UfukAntep/paintly-paint` — buraya **yalnızca exe/Mac çıktıları ve README** gider, asla kod gitmez.
**Sürüm:** 1.0.5 → 1.1.0 → 1.1.1 → **1.2.0** (kodda hazır; etiket henüz atılmadı).

---

## 1. Durum ve yapılacaklar (yeni oturumda buradan devam)

| Adım | Durum |
| :-- | :-- |
| 1.2.0 kodu, çeviriler, README | ✅ Bitti, `main`'de |
| `v1.2.0` etiketini göndermek | ⏳ **Kullanıcı yapacak** (bu ortamdan etiket gönderimi çalışmıyor) |
| exe + Mac çıktısını `paintly-paint`'e yüklemek, README'yi kopyalamak | ⏳ `publish-release.sh v1.2.0` |
| Bilgisayardaki Paintly'yi güncellemek | ⏳ `install-mac.sh` |

Kullanıcının kendi bilgisayarında, proje klasöründe çalıştıracağı komutlar:

```bash
git pull origin main && git tag v1.2.0 && git push origin v1.2.0
./scripts/publish-release.sh v1.2.0
./scripts/install-mac.sh
```

`publish-release.sh`: etiketin GitHub Actions derlemesini bekler, çıktıları indirir, README/README.tr/LICENSE'ı herkese açık depoya kopyalar ve sürümü oluşturur (kesintide yeniden dener).
Mac'te ekran görüntüsü için bir kez: **Sistem Ayarları › Gizlilik ve Güvenlik › Ekran Kaydı › Paintly**'yi aç.

**Kullanıcının kuralları**
- Kod yalnızca özel `paintly-paint-source`'a; herkese açık `paintly-paint`'e yalnızca exe/Mac çıktısı + README.
- "Bana soru sorma, tam yetki"; her özellik bitince Türkçe "X bitti" diye haber ver; bug istemiyor → her şeyi test et.
- Yeni metinler 20 dilin hepsine çevrilmeli; README İngilizce + Türkçe güncellenmeli.

---

## 2. Bu oturumda eklenen özellikler

### 1.1.0 — Paint.NET/Photoshop karşılaştırma listesi (sırayla)
1. Serbest dönüştürme: döndür, eğ, boz, perspektif (+ warp)
2. Tek tıkla arka plan silme (cihazda yapay zekâ, u2netp ONNX)
3. Uygulama içi güncelleme bildirimi
4. Düzenlenebilir yazı katmanları
5. Katman maskeleri
6. Otomatik kaydetme ve çökme kurtarma
7. İyileştirme fırçası, leke giderme
8. Kırpma aracı (oranlar, üçler kuralı, otomatik ufuk düzeltme)
9. PSD açma/kaydetme (katmanlı)
10. HEIC ve TIFF açma, TIFF kaydetme
11. Ayar katmanları
12. Nesne seçimi / Konuyu seç
13. Fırça motoru (uçlar, ön ayarlar, yumuşatma, aralık, saçılma)
14. Katman efektleri (gölge, kontur, parıltı, iç gölge, renk kaplaması)
15. Leke, Yak/Aç, Bulanıklaştır/Keskinleştir fırçaları
16. Katman grupları
17. Kalem aracı ve vektör yollar
20. Sıvılaştırma ve warp
21. Makrolar ve toplu işlem
22. Gezgin, Histogram, Bilgi panelleri
23. GIF animasyon kareleri
24. Üretken doldurma (kullanıcının kendi OpenAI anahtarıyla; anahtarsız cihazda doldurur)
25. CMYK prova, gamut uyarısı, CMYK/16-bit TIFF
26. Eklenti sistemi (yalıtılmış)

**"Yapay zekâ gibi" akıllı özellikler:** Nesneyi kaldır (içerik duyarlı doldurma), İçerik duyarlı taşıma, Portre bulanıklığı, Otomatik iyileştir, Akıllı büyüt 2×/3×/4×, İçerik duyarlı ölçekle.

**Arayüz istekleri:** Ctrl/⌘+R yeniden boyutlandırma (Paint.NET gibi), tutamaçlıyken şekil rengini değiştirme, tüm dillerde hızlı araç ipuçları, araç kutusunda **✦ Akıllı** bölümü, renk çarkı penceresi, Instagram tarzı Filtreler, başlık çubuğunda **Özellik ara** (Ctrl+K), akıllı işlemlerden sonra **Önce/Sonra** karşılaştırma çubuğu.

### 1.1.1 — Hata düzeltmesi
- "Takılı kalan araç" hatası: Akıllı düğmeler seçim yokken sessizce hiçbir şey yapmıyordu. Artık soluk görünüyor, nedenini söylüyor ve Kement aracına geçiyor.
- `publish-release.sh` çalışan derlemeyi bekliyor ve yeniden deniyor.

### 1.2.0 — 13 yeni özellik + düzeltmeler
- **Renk çarkı** artık her zaman rengarenk (parlaklık sıfırken simsiyah çıkıyordu).
- **N1 Seçimi değiştir:** genişlet, daralt, yumuşat, kenarlık, düzgünleştir, kenarı iyileştir.
- **N2 Çoklu katman seçimi:** Ctrl/⌘+tık, Shift+tık; birlikte taşı, grupla, birleştir, sil.
- **N3 Renk aralığına göre seç** (canlı önizleme).
- **N4 Kılavuzlar, yapışma, hizala/dağıt** (kılavuzlar cetvellerden sürüklenir).
- **N5 Kırpma maskesi** (Ctrl+Alt+C).
- **N6 Arka planı değiştir** (Akıllı): bulanık, renk, degrade, fotoğraf, şeffaf.
- **N7 Akıllı nesneler:** kalite kaybetmeden tekrar tekrar dönüştürme.
- **N8 Gökyüzünü değiştir** (Akıllı): 6 hazır gökyüzü veya fotoğraf, ışık uyumu.
- **N9 Portre rötuşu** (Akıllı): cihazda yüz bulma (UltraFace, MIT), cilt, göz, diş.
- **N10 Eski fotoğrafı onar** (Akıllı): toz/çizik, gren, solma, siyah-beyaz/sepya.
- **N11 Kısayol özelleştirme:** F1 penceresinde tıkla-tuşa bas, çakışma çözme, sıfırlama.
- **N12 Ekran görüntüsü al** (Ctrl+Alt+Shift+S): ekran/pencere, gecikme, Paintly'yi gizle, bölge kırpma.
- **N13 Eğri yazı / yolda yazı:** kavis veya kalem yolu boyunca, düzenlenebilir.
- 146 yeni metin 18 dile çevrildi (toplam 20 dil); README (EN+TR) güncellendi.

---

## 3. Teknik notlar (geliştirici için)

- **Yapı:** Electron (`electron/main.cjs`, `preload.cjs` → `window.paintly`), Vite, TypeScript, Canvas 2D, çerçevesiz.
- **Belge modeli** (`src/core/document.ts`): düz katman dizisi + `parent` (gruplar); `structural()` / `pushPixels()` geçmiş adımları; `renderItems`/`layerContent` birleştirme (grup, kırpma, efekt, ayar katmanı); `selectedIds` çoklu seçim; `guides`.
- **Katman** (`src/core/layer.ts`): `kind` raster/text/adjustment, `mask`, `clip`, `smart {source, quad, warp}`, `text` (`TextData`, `curve` alanı).
- **Yapay zekâ** (`src/ai/`): `segment.ts` (u2netp + `loadModel()` + guided filter), `face.ts` (UltraFace RFB-320), `inpaint.ts` (PatchMatch), `sky.ts`, `retouch.ts`, `restore.ts`, `enhance.ts`, `portrait.ts`. Modeller `public/models/` (lisanslar `NOTICE.txt`); ORT wasm `ort/` altına kopyalanır, Electron'da `asset:read` IPC ile okunur.
- **Eylemler:** `src/actions.ts` (`ACTIONS`, kısayollar `keys`), menüler `src/ui/menubar.ts`, Akıllı bölüm `SMART_LAYOUT` (`src/tools/index.ts`), diyaloglar `src/ui/aiDialogs.ts` / `dialogs.ts`, kısayol kaydı `src/shortcuts.ts` (localStorage `paintly.shortcuts.v1`), ekran görüntüsü `src/ui/capture.ts` + `capture:sources/grab` IPC.
- **Çeviri:** `src/i18n/locales/*.json`; yeni anahtar → önce en+tr, sonra 18 dile çeviri.
- **Test yöntemi:** Vite + Playwright ile tarayıcıda betikler (tüm araçlar, 22 eylem, 80 efekt, geri al/yinele, 11 kayıt biçimi); üretim testi `xvfb-run` + Playwright `_electron`. Son durumda regresyon testi hatasız.
- **Bilinen notlar:**
  - Ekran görüntüsü sanal ekranda (xvfb) bazen boş liste veriyordu → ekranlar/pencereler ayrı isteniyor, yeniden deneniyor. Gerçek Windows/Mac'te ayrıca denenmedi.
  - Portre rötuşu yüz kutusuna göre göz/ağız buluyor; yüz bulunamazsa uyarı verir.
  - Etiket gönderimi bu bulut ortamından çalışmıyor; GitHub Actions `workflow_dispatch` çalışıyor.
