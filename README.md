# Müşteri Takip Uygulaması

Patates ve sarı patates siparişlerini müşteri bazında takip eden basit bir web uygulaması.

- Müşteri adı + tarih
- İki tablo: **Patates** ve **Sarı Patates**
- Her satır: sipariş kg · gelen kg · fark · birim fiyat · tutar
- Gelen kg siparişten farklıysa satır **kırmızı** gösterilir
- Otomatik toplam ve genel toplam
- **Excel** ve **PDF** olarak indirme
- Telefonda "Ana ekrana ekle" ile uygulama gibi çalışır (PWA, çevrimdışı destekli)

## Yayınlama (GitHub Pages)

1. Bu klasördeki dosyaları bir GitHub deposuna yükle
2. Depo → **Settings → Pages** → Branch: `main`, klasör: `/ (root)` → **Save**
3. Birkaç dakika sonra `https://<kullanici-adi>.github.io/<depo-adi>/` adresinde yayında

## Dosyalar

| Dosya | Açıklama |
|---|---|
| `index.html` | Uygulamanın tamamı (HTML + CSS + JS) |
| `manifest.webmanifest` | PWA tanımı (ikon, isim, renk) |
| `sw.js` | Service worker — çevrimdışı çalışma |
| `icons/` | Uygulama ikonları (192 / 512 px) |

Veriler kullanıcının tarayıcısında (`localStorage`) saklanır; sunucuya gönderilmez.
