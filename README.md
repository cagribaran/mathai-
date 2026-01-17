# MathAI - PWA Kurulum Rehberi 📱

MathAI'yi iPhone'una yüklemek için bu adımları takip et!

## 🚀 Kurulum Adımları

### 1. Dosyaları Bir Web Sunucusuna Yükle

PWA'ların çalışması için HTTPS gerekir. En kolay yöntemler:

#### Seçenek A: GitHub Pages (Ücretsiz & Kolay) ⭐ ÖNERİLEN

1. GitHub'da yeni bir repository oluştur (örn: `mathai`)
2. Tüm dosyaları repository'ye yükle:
   - index.html
   - manifest.json
   - service-worker.js
   - icon-192.png
   - icon-512.png

3. Settings → Pages'e git
4. Source: "Deploy from a branch" seç
5. Branch: "main" seç
6. Save'e tıkla

5-10 dakika içinde siteniz hazır! URL: `https://[kullanıcı-adın].github.io/mathai`

#### Seçenek B: Netlify (Hızlı & Kolay)

1. [netlify.com](https://netlify.com)'a git
2. "Add new site" → "Deploy manually"
3. Tüm dosyaları sürükle-bırak
4. Otomatik deploy edilecek!

#### Seçenek C: Vercel

1. [vercel.com](https://vercel.com)'a git
2. "New Project" → dosyaları yükle
3. Deploy!

### 2. iPhone'a Yükleme

1. **Safari ile aç** (Chrome değil!)
2. Sitenin URL'sini ziyaret et
3. **Paylaş** butonuna bas (⬆️ işareti)
4. **"Ana Ekrana Ekle"** seçeneğini bul
5. İsmi düzenle (isterseniz)
6. **"Ekle"** butonuna bas

🎉 **Tebrikler!** Artık MathAI ana ekranında gerçek bir uygulama gibi!

## 📱 PWA Özellikleri

- ✅ Ana ekranda kendi ikonu
- ✅ Tam ekran mod (tarayıcı barı yok)
- ✅ Hızlı başlatma
- ✅ Offline çalışma desteği
- ✅ Otomatik güncellemeler

## 🛠️ Yerel Test (Opsiyonel)

Yüklemeden önce test etmek istersen:

```bash
# Python ile basit sunucu
python3 -m http.server 8000

# Node.js varsa
npx serve
```

Sonra `http://localhost:8000` adresinden test et.

**ÖNEMLİ:** iPhone'da PWA yüklemek için HTTPS gerekir, bu yüzden yerel test sadece bilgisayarda çalışır.

## 🔧 Sorun Giderme

### "Ana Ekrana Ekle" seçeneği görünmüyor
- Safari kullandığından emin ol (Chrome'da olmaz)
- HTTPS ile açtığından emin ol
- Zaten yüklüyse sitenin aynısını tekrar yükleyemezsin

### Uygulama açılmıyor
- Sitenin hala aktif olduğunu kontrol et
- Uygulamayı sil ve tekrar yükle
- Safari'nin cache'ini temizle

### API çalışmıyor
- İnternet bağlantını kontrol et
- Claude API'nin erişilebilir olduğundan emin ol

## 📝 Notlar

- PWA, normal web uygulamasıyla aynı özelliğe sahip
- Apple Developer hesabı gerekmez
- Tamamen ücretsiz
- İstediğin kadar güncelleme yapabilirsin
- Silmek istersen normal uygulama gibi silebilirsin

## 🎨 Özelleştirme

`manifest.json` dosyasını düzenleyerek:
- Uygulama ismini değiştirebilirsin
- Tema rengini ayarlayabilirsin
- Açılış yönünü belirleyebilirsin

## 📮 Destek

Sorun yaşarsan:
1. Tarayıcı konsolunu kontrol et (Safari → Geliştirici → Console)
2. Service Worker'ın kayıtlı olduğunu kontrol et
3. Manifest dosyasının doğru yüklendiğini kontrol et

---

**Keyifli kullanımlar! 🎓✨**
