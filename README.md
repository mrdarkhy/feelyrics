# Feelyrics

Şarkı sözlerini kelimesi kelimesine değil, olabilecek en yakın **his**le çeviren
transcreation player'ı — *his > anlam > kelime*.

**Canlı sayfa:** GitHub Pages'i açınca `https://<kullanici>.github.io/feelyrics/` adresinde.

## Nasıl çalışır
- `index.html` tek dosyadır; sunucu ve veritabanı yoktur.
- Paylaşılan şarkılar linkin `#f1.` kısmında sıkıştırılmış olarak taşınır
  (deflate + base64url; emsal: mermaid.live, Excalidraw). **Söz metni hiçbir sunucuya gönderilmez.**
- Sayfada önyüklü tek tam şarkı, sözleri kamu malı olan Guantanamera'dır (José Martí, 1891).
  Telifli sözler repo'ya **eklenmez** — bkz. CONTRIBUTING.

## Kurulum (bir kez)
1. Bu klasörü GitHub'da yeni bir repo'ya push'la (örn. `feelyrics`).
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)` → Save.
3. Birkaç dakika içinde site yayında.

## Katkı ve roller (Wikipedia modeli, sıfır backend)
- **Herkes:** şarkı isteği → Issue ("İstek şarkı" şablonu); satır düzeltmesi → Pull Request.
- **Onay:** hiçbir değişiklik onaysız siteye girmez — PR'ları maintainer onaylar.
- **Güvenilen doğrulayıcılar:** isabetli PR'ları kabul edilenler *collaborator* yapılır
  ve doğrudan editleyebilir (rol merdiveni: Dinleyici → Doğrulayıcı → Uzman → Küratör).

## Yol haritası
- v2: şarkı verilerinin `songs/*.json` dosyalarına ayrılması (PR'lar daha temiz diff verir)
- PWA manifest'i (telefonda "ana ekrana ekle")
- Üyelikli doğrulayıcı akışı (satır durum-makinesi: AI-taslak → önerildi → oturdu → disputed → küratör)

Lisans: henüz seçilmedi (repo sahibinin kararı).
