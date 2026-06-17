 🛍️ Mini Katalog Uygulaması

Flutter ile geliştirilmiş, gerçek API verisiyle çalışan ürün listeleme ve sepet yönetimi sunan mobil katalog uygulaması.

---

 📱 Ekran Görüntüleri

![Uygulama Ekranları](screenshoots.png)

*Sol'dan sağa: Ana Sayfa · Boş Sepet · Dolu Sepet · Ürün Detayı*

---

✨ Özellikler

- 🔍 Anlık arama ve kategori filtresi
- 📦 GridView ile ürün listeleme
- 📄 Ürün detay sayfası (açıklama, özellikler, puan)
- 🛒 Sepet yönetimi — ürün ekleme, çıkarma, adet güncelleme
- 🌐 Fake Store API entegrasyonu ile gerçek veri
- 🎨 Temiz beyaz tema


🛠️ Kullanılan Teknolojiler

| Araç | Versiyon |
|------|----------|
| Flutter SDK | 3.x |
| Dart SDK | ≥ 3.0.0 |
| `http` paketi | ^1.2.0 |
| `cached_network_image` | ^3.3.1 |
| Fake Store API | [fakestoreapi.com](https://fakestoreapi.com/products) |

---

 🚀 Çalıştırma Adımları

 1. Gereksinimleri kur

Flutter ve Android Studio kurulu olmalıdır:
- Flutter: https://flutter.dev/docs/get-started/install
- Android Studio (Emülatör için): https://developer.android.com/studio

 2. Projeyi klonla

```bash
git clone https://github.com/KULLANICI_ADINIZ/mini_katalog.git
cd mini_katalog
```

 3. Bağımlılıkları yükle

```bash
flutter pub get
```

 4. Emülatörü başlat

Android Studio üzerinden bir sanal cihaz (AVD) oluşturup başlatın,  
ya da fiziksel bir Android cihazı USB ile bağlayın.

 5. Uygulamayı çalıştır

```bash
flutter run
```

---

📁 Proje Yapısı

```
lib/
├── main.dart                        # Uygulama giriş noktası & Named Routes
├── models/
│   ├── product.dart                 # Ürün modeli (fromJson / toJson)
│   └── cart_item.dart               # Sepet öğesi modeli
├── services/
│   ├── api_service.dart             # HTTP istekleri — Fake Store API
│   └── cart_service.dart            # Sepet state yönetimi (Singleton)
├── screens/
│   ├── home_screen.dart             # Ana sayfa — GridView ürün listesi
│   ├── product_detail_screen.dart   # Ürün detay sayfası
│   └── cart_screen.dart             # Sepet ekranı
├── widgets/
│   ├── product_card.dart            # Yeniden kullanılabilir ürün kartı
│   ├── cart_badge.dart              # Sepet ikonu + adet rozeti
│   └── category_chip.dart          # Kategori filtre chip'i
└── theme/
    └── app_theme.dart               # Merkezi renk ve tema tanımları
```

---

 📚 Öğrenilen Konular

Bu proje aşağıdaki Flutter konularını kapsamaktadır:

- `StatelessWidget` & `StatefulWidget` kullanımı
- `Navigator.push` / `pop` ile sayfa geçişleri
- `Route Arguments` ile sayfalar arası veri taşıma
- `ListView.builder` & `GridView.builder` ile dinamik listeler
- JSON verisi ve `fromJson` / `toJson` model sınıfı
- `http` paketi ile REST API çağrısı
- Singleton pattern ile state yönetimi
- Arama ve filtreleme mantığı

---

 👤 Geliştirici

> Barış Kaya 

