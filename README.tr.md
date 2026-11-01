<div align="center">

<img src="docs/banner.svg" alt="Paintly Paint" width="100%">

<br>

**Klasik Paint ve Paint.NET'te sevdiğin her şey, tek bir tatlı ve ücretsiz uygulamada.**
Katmanlar, 60'tan fazla efekt ve ayarlama, değnek, degradeler, metin, şekiller, sınırsız geri alma ve 20 dil.

<br>

[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-8b5cf6?style=for-the-badge&logo=windows11&logoColor=white)](../../releases/latest)
[![macOS](https://img.shields.io/badge/macOS-Apple%20Silicon%20%26%20Intel-ec4899?style=for-the-badge&logo=apple&logoColor=white)](../../releases/latest)
[![Lisans](https://img.shields.io/badge/lisans-ücretsiz%20·%20indir%20%26%20kullan-a855f7?style=for-the-badge)](LICENSE.md)
[![Diller](https://img.shields.io/badge/dil-20-f472b6?style=for-the-badge&logo=googletranslate&logoColor=white)](#-20-dil)
[![Bağış](https://img.shields.io/badge/❤-Bağış%20Yap-ff69b4?style=for-the-badge)](#-paintlyye-destek-ol)

[**⬇️ İndir**](#%EF%B8%8F-i̇ndir) · [**✨ Özellikler**](#-özellikler) · [**⌨️ Kısayollar**](#%EF%B8%8F-klavye-kısayolları) · [**💜 Bağış**](#-paintlyye-destek-ol) · [**🇬🇧 English**](README.md)

</div>

<br>

<p align="center">
  <img src="docs/screenshot-light.jpg" alt="Paintly Paint — açık tema" width="92%">
</p>

---

## ⬇️ İndir

En son sürümü **[Releases sayfasından](../../releases/latest)** indir.

| Platform | Dosya | Not |
| :-- | :-- | :-- |
| 🪟 **Windows 10 / 11** | `PaintlyPaint-x.y.z-win-setup.exe` | Kurulum sihirbazı, masaüstü kısayolu dahil |
| 🪟 **Windows taşınabilir** | `PaintlyPaint-x.y.z-win-portable.exe` | Kurulum gerektirmez, USB bellekten çalışır |
| 🍎 **macOS** (Apple Silicon) | `PaintlyPaint-x.y.z-mac-arm64.dmg` | M1 / M2 / M3 / M4 Mac'ler |
| 🍎 **macOS** (Intel) | `PaintlyPaint-x.y.z-mac-x64.dmg` | Intel işlemcili Mac'ler |

### 🍎 macOS'a kurulum

1. İndirdiğin `.dmg` dosyasını aç.
2. Açılan pencerede **Paintly Paint'i Uygulamalar (Applications) klasörüne sürükle**. Doğrudan disk görüntüsünün içinden çalıştırma.
3. Paintly Paint'i **Launchpad**'den veya **Uygulamalar** klasöründen aç.

İlk açılışta macOS şu uyarıyı gösterir:

> *Apple, "Paintly Paint" öğesinin Mac'inize zarar verebilecek veya gizliliğinizi ihlal edebilecek bir kötü amaçlı yazılım içermediğini doğrulayamadı.*

**Bu uyarı neden çıkıyor?** Apple bu uyarıyı yalnızca Apple Developer Program'a (yıllık 99 $) üye olan ve her sürümünü Apple'a kontrol ettiren ("notarization") geliştiricilerin uygulamalarında göstermiyor. Paintly Paint ücretsiz bir hobi projesi ve henüz bu onaydan geçmedi, bu yüzden macOS uygulamaya kefil olamıyor. Uygulama güvenli: hiçbir veri toplamaz, internete bağlanmaz, sadece senin seçtiğin resim dosyalarını açıp kaydeder.

**Yine de açmak için (bir kez yeterli):**

1. Uyarıda **Bitti**'ye tıkla. Uygulamayı Çöp Sepeti'ne taşıma.
2. **Sistem Ayarları → Gizlilik ve Güvenlik**'i aç.
3. Aşağı kaydır, *"Paintly Paint" engellendi…* yazısının yanındaki **Yine de Aç**'a tıkla.
4. Şifreni veya Touch ID'ni gir, ardından **Aç**'a tıkla.

**Ya da Terminal ile (tek komut):**

```bash
xattr -cr "/Applications/Paintly Paint.app"
```

Tarayıcı indirdiğin her dosyaya "internetten indirildi" işareti (*karantina* işareti) koyar; uyarıyı çıkaran şey bu işarettir. Bu komut işareti sadece Paintly Paint'ten kaldırır. Mac'indeki başka hiçbir güvenlik ayarını değiştirmez.

> [!TIP]
> Terminal `No such file` derse uygulama henüz Uygulamalar klasöründe değildir. Önce yukarıdaki 2. adımı yap.
>
> macOS uygulama için **"hasarlı / bozuk"** derse büyük ihtimalle 1.0.0 sürümünü indirmişsindir. Bunun yerine [en son sürümü](../../releases/latest) indir.

### 🪟 Windows'a kurulum

`PaintlyPaint-x.y.z-win-setup.exe` dosyasını (ya da taşınabilir `.exe`'yi) çalıştır. Windows SmartScreen *"Windows bilgisayarınızı korudu"* diyebilir. Sebebi macOS'takiyle aynı: uygulama ücretli bir kod imzalama sertifikasıyla imzalanmadı. **Ek bilgi → Yine de çalıştır**'a tıkla.

---

## ✨ Özellikler

<table>
<tr>
<td width="50%" valign="top">

### 🎨 Çizim ve boyama
- 7 fırça tipi: yuvarlak, kaligrafi, keçeli kalem, pastel boya, yağlı boya, suluboya, doğal kurşun kalem
- **Boyut, sertlik, kenar yumuşatma** ve **karışım modu** ayarları
- Piksel hassasiyetinde **Kurşun Kalem**, yumuşak **Sprey**, **Silgi** (sağ tık ikincil renkle boyar)
- Toleranslı, bitişik/genel dolgulu **Boya Kovası**
- **Degrade**: doğrusal, yansıyan, dairesel, elmas, konik ve şeffaflık modu
- **Klon Damgası** ve **Yeniden Renklendir**
- 1 / 3×3 / 5×5 / 9×9 örneklemeli **Renk Seçici**
- Basınca duyarlı kalem desteği ✍️

</td>
<td width="50%" valign="top">

### 🔷 Şekiller, çizgiler ve metin
- **22 şekil**: dikdörtgen, yuvarlak köşeli dikdörtgen, elips, üçgen, çokgenler, yıldızlar, oklar, kalp, bulut, konuşma balonu, şimşek…
- Kontur / dolgu / kontur + dolgu, kesikli ve noktalı çizgiler
- Şekiller onaylanana kadar **tutamaçlarla düzenlenebilir**
- Paint usulü bükülebilen **Çizgi / Eğri** aracı ve ok uçları
- Her yazı tipiyle **Metin**: boyut, kalın, italik, altı çizili, üstü çizili, hizalama

</td>
</tr>
<tr>
<td valign="top">

### ✂️ Seçimler
- **Dikdörtgen**, **Elips**, **Kement** ve **Değnek**
- Değiştir, ekle, çıkar, kesişim, xor modları
- Hareketli "karınca" kenarlıklar 🐜
- Tutamaçlarla boyutlandırılabilen **Seçili Pikselleri Taşı**
- Seçime kırp, seçimi sil / doldur, seçimi tersine çevir

</td>
<td valign="top">

### 🧅 Katmanlar
- Küçük resimli, sınırsız katman
- Opaklık, görünürlük ve **18 karışım modu**
- Ekle, sil, çoğalt, aşağı birleştir, düzleştir, sürükleyerek sırala
- Dosyadan katman olarak içe aktar
- Katmanı çevir, **döndür / yakınlaştır**

</td>
</tr>
<tr>
<td valign="top">

### 🪄 Ayarlamalar (14)
Otomatik Seviye · Siyah Beyaz · Parlaklık / Kontrast · Eğriler · Ton / Doygunluk · Renkleri Ters Çevir · Seviyeler · Posterleştir · Sepya · Eşik · Canlılık · Sıcaklık / Renk Tonu · Pozlama · Renk Dengesi

</td>
<td valign="top">

### 🌈 Efektler (47)
- **Sanatsal:** Mürekkep Eskiz, Yağlı Boya, Kurşun Kalem Eskiz, Karikatür, Suluboya
- **Bulanıklık:** Gauss, Hareket, Dairesel, Yakınlaştırma, Odak Dışı, Yüzey, Parça, Kutu
- **Bozma:** Şişirme, Burgu, Pikselleştir, Buzlu Cam, Göçük, Karo Yansıma, Kutupsal Ters Çevirme, Dalga, Kristalize
- **Gürültü:** Gürültü Ekle, Medyan, Gürültü Azalt, Leke Giderme
- **Fotoğraf:** Parıltı, Keskinleştir, Keskinlik Maskesi, Portre Yumuşatma, Kırmızı Göz Giderme, Vinyet, Tilt-Shift, Rüya
- **Oluştur:** Bulutlar, Julia ve Mandelbrot fraktalları, Plazma, Dama Tahtası
- **Stilize:** Kenar Bul, Kabartma, Anahat, Rölyef, Sobel, Solarize, Yarım Ton, Neon Parıltı

Her efektte **canlı önizleme** var.

</td>
</tr>
<tr>
<td valign="top">

### 🖼️ Resim ve dosyalar
- **PNG, JPG, BMP, GIF, WebP, ICO, SVG, AVIF** açar
- **PNG, JPG, WebP, BMP, ICO** veya katmanlı **`.ppaint`** proje formatında kaydeder
- Yeniden boyutlandır, tuval boyutu (çapa ile), otomatik kırp
- Çevir ve 90° / 180° döndür
- **Sekmelerde** birden fazla resim, sürükle-bırak ile açma
- Sistem panosuyla kopyala / yapıştır, yeni katmana veya yeni resme yapıştır
- Yazdır

</td>
<td valign="top">

### 💖 Göze hoş gelsin diye
- **Açık ve koyu tema**, 8 vurgu rengiyle pastel arayüz
- Her yerde yaylı animasyonlar ve küçük bir açılış ekranı 🎉
- Tıklanabilir **Geçmiş** paneliyle sınırsız **geri al / yinele**
- %1–%6400 yakınlaştırma, piksel ızgarası, cetveller, trackpad ile yakınlaştırma
- Windows'ta (Ctrl) ve macOS'ta (⌘) doğal kısayollar

</td>
</tr>
</table>

<p align="center">
  <img src="docs/screenshot-dark.jpg" alt="Koyu tema" width="49%">
  <img src="docs/screenshot-effects.jpg" alt="Canlı önizlemeli efekt" width="49%">
</p>

---

## 🌍 20 dil

Paintly Paint sistem dilini otomatik algılar. Dili istediğin zaman **Yardım → Ayarlar** menüsünden değiştirebilirsin.

| | | | |
| :-- | :-- | :-- | :-- |
| 🇬🇧 English | 🇹🇷 Türkçe | 🇩🇪 Deutsch | 🇫🇷 Français |
| 🇪🇸 Español | 🇮🇹 Italiano | 🇧🇷 Português (Brasil) | 🇳🇱 Nederlands |
| 🇵🇱 Polski | 🇨🇿 Čeština | 🇸🇪 Svenska | 🇷🇺 Русский |
| 🇺🇦 Українська | 🇸🇦 العربية | 🇮🇳 हिन्दी | 🇮🇩 Bahasa Indonesia |
| 🇻🇳 Tiếng Việt | 🇨🇳 简体中文 | 🇯🇵 日本語 | 🇰🇷 한국어 |

Bir çeviri hatası mı gördün? [Issue açıp](../../issues) haber verirsen çok sevinirim 💜

---

## ⌨️ Klavye kısayolları

Windows'taki `Ctrl`, macOS'ta `⌘` demektir. Tam liste için uygulamada **F1**'e bas.

| Araç | Tuş | | Komut | Kısayol |
| :-- | :-: | :-- | :-- | :-- |
| Seçim araçları (sırayla) | `S` | | Yeni / Aç / Kaydet | `Ctrl` `N` / `O` / `S` |
| Taşıma araçları | `M` | | Geri al / Yinele | `Ctrl` `Z` / `Ctrl` `Y` (`⌘⇧Z`) |
| Yakınlaştır / Kaydır | `Z` / `H` | | Kopyala / Yapıştır | `Ctrl` `C` / `V` |
| Kurşun kalem / Fırça | `P` / `B` | | Yeni katmana yapıştır | `Ctrl` `Shift` `V` |
| Sprey / Silgi | `A` / `E` | | Tümünü seç / Seçimi kaldır | `Ctrl` `A` / `Ctrl` `D` |
| Boya kovası / Degrade | `F` / `G` | | Seçime kırp | `Ctrl` `Shift` `X` |
| Renk seçici | `K` | | Yeniden boyutlandır / Tuval boyutu | `Ctrl` `E` / `Ctrl` `Shift` `R` |
| Klon damgası / Yeniden renklendir | `L` / `R` | | Yeni katman | `Ctrl` `Shift` `N` |
| Metin | `T` | | Yakınlaştır / Uzaklaştır / Sığdır | `Ctrl` `+` / `-` / `B` |
| Çizgi, Şekiller | `O` | | Son efekti tekrarla | `Ctrl` `F` |
| Fırça boyutu − / + | `[` / `]` | | Renkleri değiştir | `X` |
| Her yerde kaydır | `Boşluk` + sürükle | | Bitir / iptal | `Enter` / `Esc` |

---

## 💜 Paintly'ye destek ol

Paintly Paint **tamamen ücretsiz**: reklam yok, takip yok. Hoşuna gittiyse küçük bir bağışla teşekkür edebilirsin. Her katkı yeni özellikler geliştirmeme yardım ediyor ✨

Uygulamanın sağ üstündeki **❤ Bağış Yap** düğmesine tıklayınca hesap bilgileri tek tıkla kopyalanabilir şekilde açılır.

<!-- DONATE:START -->
<div align="center">

**Uluslararası banka havalesi (SWIFT)**: USD ve EUR hesapları.
Bilgiler uygulamadaki **Bağış** penceresinde.

</div>
<!-- DONATE:END -->

Bağış yapamıyor musun? Repoya ⭐ **yıldız vermek** de çok yardımcı olur!

---

## 📜 Lisans

**İndir ve kullan; değiştirme, paylaşma.** Paintly Paint ücretsiz bir yazılımdır (freeware) ve [**Paintly Paint Freeware Lisansı**](LICENSE.md) ile sunulur.

| ✅ Serbest | ❌ Yasak |
| :-- | :-- |
| [Resmî Releases sayfasından](../../releases/latest) ücretsiz indirmek | Uygulamayı değiştirmek, kaynak kodunu çıkarmak |
| Kişisel, eğitim ve kâr amacı gütmeyen kullanım | Uygulama dosyalarını paylaşmak veya başka yere yüklemek. Bunun yerine resmî linki paylaş 🙂 |
| **Kendi çizdiğin resimleri** her amaçla, **ticari olarak bile** kullanmak 🎨 | **Uygulamayı satmak** veya ticari bir ürünün parçası yapmak |
| Resmî linkle arkadaşlarına önermek | Lisans veya telif bildirimlerini kaldırmak |

Paintly Paint ile **senin çizdiğin resimler** tamamen sana aittir; ticari dahil istediğin gibi kullanabilirsin.
Başka bir izin için lütfen [issue aç](../../issues).

<div align="center">
<br>

💜 ve bolca 🎨 ile yapıldı

<sub>Paintly Paint bağımsız bir projedir; Microsoft veya dotPDN LLC ile bağlantılı değildir.</sub>

</div>
