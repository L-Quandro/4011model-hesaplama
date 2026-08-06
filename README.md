# 4011 Model Hesaplama (PWA)

Tren makinistleri için iki zaman arası fark hesaplama ve çoklu saat toplama aracı. Artık bir **PWA (Progressive Web App)** — telefona "uygulama gibi" yüklenebilir, tam ekran açılır ve internet olmadan da çalışır.

## GitHub Pages ile yayınlama

1. Bu klasördeki tüm dosyaları (`index.html`, `manifest.json`, `sw.js`, `icons/`) bir GitHub reposuna yükleyin.
2. Repo **Settings → Pages** bölümüne gidin.
3. **Source** olarak `main` branch ve `/ (root)` klasörünü seçip **Save**'e basın.
4. Birkaç dakika sonra siteniz `https://kullaniciadiniz.github.io/repo-adi/` adresinde yayında olacak.

## Telefona yükleme

- **Android (Chrome):** Siteyi açın → sağ üstteki ⋮ menüsü → "Ana ekrana ekle" / "Uygulamayı yükle".
- **iPhone (Safari):** Siteyi açın → Paylaş butonu (⬆️) → "Ana Ekrana Ekle".

Yüklendikten sonra tarayıcı çubuğu olmadan, tam ekran bir uygulama gibi açılır ve ikon olarak tren + saat rozetli özel ikon görünür.

## Dosya yapısı

```
index.html          → Ana uygulama (hesaplama araçları)
manifest.json        → PWA kimlik bilgileri (isim, ikon, renkler)
sw.js                 → Service worker (çevrimdışı çalışma desteği)
icons/icon-192.png    → Uygulama ikonu (küçük)
icons/icon-512.png    → Uygulama ikonu (büyük)
icons/icon-maskable-512.png → Android adaptif ikon
```

## Not

`start_url` ve `scope` göreli (relative) yollarla ayarlandığı için, repo adını alt dizin (`/repo-adi/`) olarak kullanan GitHub Pages yapısında sorunsuz çalışır. Dosyaları taşımadığınız sürece ek bir ayar gerekmez.
