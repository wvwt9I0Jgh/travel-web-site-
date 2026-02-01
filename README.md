# BU PROJE DOSYALAI ÇOK BÜYÜK OLDUĞUNDAN DOLAYI COMMİT SIRASINDA AKSAKLIK YAŞANMIŞTIR


# EliteLux Premium Limousine Services - Full Project Documentation

## 📋 Proje Genel Bakış

Bu proje, **EliteLux Premium Limousine Services** için geliştirilmiş kapsamlı bir web platformu ve admin panel sistemidir. PHP, MySQL, Bootstrap ve TinyMCE teknolojileri kullanılarak geliştirilmiştir. Proje iki ana website ve güçlü bir CMS admin panel içermektedir.

## 🏗️ Proje Yapısı

### Ana Dizin Yapısı

```
aa/
├── README.md                    # Ana proje dokümantasyonu
├── view.php                     # Genel sayfa görüntüleyici
├── project_status_final.php     # Proje durum kontrolü
├── travel_admin_panel.html      # Admin panel ana sayfası
├── test_*.php                   # Sistem test dosyaları
├── 
├── a/                           # Ana geliştirme klasörü
│   ├── admin.php               # Admin panel giriş noktası
│   ├── view.php                # Sayfa görüntüleyici
│   ├── config/                 # Konfigürasyon dosyaları
│   ├── includes/               # Ortak dosyalar
│   ├── admin/                  # Admin panel modülleri
│   ├── websitem/               # Ana website
│   ├── websitelerim/           # İkinci website
│   ├── modules/                # HTML modülleri
│   ├── php/                    # PHP fonksiyonları
│   ├── css/                    # Stil dosyaları
│   ├── js/                     # JavaScript dosyaları
│   └── tinymce_8.0.2_dev/      # TinyMCE editör
│
├── websitem/                   # Ana website kopyası
├── websitelerim/               # İkinci website kopyası
├── admin/                      # Admin panel kopyası
├── css/                        # Stil dosyaları
├── js/                         # JavaScript dosyaları
└── php/                        # PHP fonksiyonları
```

## 🌟 Ana Özellikler

### 1. **Multi-Website Sistemi**

#### 🏢 EliteLux Ana Website (`websitem/`)
- **Ana sayfa**: Premium limuzin hizmetleri tanıtımı
- **Hizmetler**: Kurumsal transfer, havaalanı transferi, özel etkinlik transportu
- **Filo**: Lüks araç koleksiyonu
- **Rezervasyon**: Çevrimiçi rezervasyon sistemi
- **İletişim**: Müşteri iletişim formu
- **Responsive tasarım**: Tüm cihazlarda uyumlu

#### 🚗 EliteLux İkinci Website (`websitelerim/`)
- Ana website'in alternatif versiyonu
- Aynı özellikler farklı tasarım yaklaşımıyla
- Bağımsız içerik yönetimi
- Farklı hedef kitle için özelleştirilmiş

### 2. **Güçlü CMS Admin Panel**

#### 📊 Dashboard Özellikleri
- **Gerçek zamanlı istatistikler**: Rezervasyonlar, mesajlar, blog yazıları
- **Son aktiviteler**: Her iki website'den güncellemeler
- **Hızlı işlemler**: Tek tıkla önemli fonksiyonlara erişim
- **Multi-folder görünüm**: websitem ve websitelerim dosyaları
- **Responsive admin paneli**: Mobil uyumlu yönetim

#### 📄 Sayfa Yönetimi (Multi-Folder CMS)
- **Çift klasör desteği**: websitem ve websitelerim için ayrı yönetim
- **TinyMCE Editör**: Görsel içerik editörü
- **Otomatik dosya oluşturma**: CMS'den PHP dosyası otomatik üretimi
- **Preview sistemi**: Yayınlama öncesi önizleme
- **SEO optimizasyonu**: Meta tags, anahtar kelime yönetimi
- **Dosya senkronizasyonu**: Veritabanı ↔ Dosya sistemi entegrasyonu

#### 🚗 Araç Yönetimi
- **Araç kategorileri**: Sedan, SUV, Limuzin, VIP
- **Fiyat yönetimi**: Dinamik fiyatlandırma sistemi
- **Fotoğraf yükleme**: Çoklu görsel yönetimi
- **Özellik tanımlama**: Araç detayları ve kapasitesi

#### 📅 Rezervasyon Sistemi
- **Rezervasyon takibi**: Durum yönetimi (Beklemede, Onaylandı, İptal)
- **Müşteri bilgileri**: Detaylı müşteri profilleri
- **Tarih/saat yönetimi**: Çakışma kontrolü
- **Ödeme takibi**: Ödeme durumu ve tutar yönetimi
- **Otomatik e-mail**: Rezervasyon onay mailiIeri

#### 💬 İletişim Yönetimi
- **Mesaj kutusu**: Website formlarından gelen mesajlar
- **Okundu/okunmadı**: Mesaj durumu takibi
- **Yanıtlama sistemi**: E-mail entegrasyonu
- **Kategorizasyon**: Mesaj türlerine göre sınıflandırma

#### 📝 Blog Sistemi
- **Blog yazı editörü**: TinyMCE ile zengin editör
- **Kategori yönetimi**: Çok kategorili yazı sistemi
- **Yorum sistemi**: Kullanıcı yorumları ve moderasyon
- **SEO optimizasyonu**: Blog için özel SEO araçları
- **Sosyal medya paylaşım**: Otomatik sosyal medya entegrasyonu

### 3. **Teknik Özellikler**

#### 🗄️ Veritabanı Yapısı
- **travel_agency** veritabanı
- **Ana tablolar**:
  - `admin_users`: Admin panel kullanıcıları
  - `cms_pages`: CMS sayfaları (multi-folder)
  - `vehicles`: Araç bilgileri
  - `vehicle_categories`: Araç kategorileri
  - `bookings`: Rezervasyonlar
  - `messages`: İletişim mesajları
  - `blog_posts`: Blog yazıları
  - `blog_categories`: Blog kategorileri
  - `users`: Website kullanıcıları

#### 🔐 Güvenlik Özellikleri
- **Password hashing**: PHP password_hash() kullanımı
- **Session yönetimi**: Güvenli oturum kontrolü
- **CSRF koruması**: Cross-site request forgery koruması
- **SQL injection koruması**: Prepared statements
- **XSS koruması**: Output sanitization

#### ⚡ Performans Optimizasyonu
- **Dosya cache sistemi**: Statik dosya önbellekleme
- **Database optimizasyonu**: İndeksli veritabanı yapısı
- **Image optimization**: Otomatik resim sıkıştırma
- **Minified assets**: CSS ve JavaScript sıkıştırma

## 🚀 Kurulum ve Yapılandırma

### Gereksinimler
- **PHP**: 8.0 veya üzeri
- **MySQL**: 5.7 veya üzeri
- **Web Server**: Apache veya Nginx
- **XAMPP/WAMP**: Yerel geliştirme için

### Kurulum Adımları

1. **Dosyaları Kopyalama**
   ```bash
   # Projeyi XAMPP htdocs klasörüne kopyalayın
   C:\xampp\htdocs\aa\
   ```

2. **Veritabanı Kurulumu**
   ```php
   # Veritabanını otomatik oluşturmak için
   http://localhost/aa/a/admin/recreate_database.php
   ```

3. **Konfigürasyon**
   ```php
   # config/database.php dosyasını düzenleyin
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "travel_agency";
   ```

4. **Admin Kullanıcı Oluşturma**
   ```php
   # İlk admin kullanıcısını oluşturun
   http://localhost/aa/a/admin/create_admin_user.php
   ```

## 📱 Kullanım Kılavuzu

### Admin Panel Giriş
```
URL: http://localhost/aa/a/admin.php
Kullanıcı: admin
Şifre: admin123
```

### Website Erişimi
```
Ana Website: http://localhost/aa/websitem/
İkinci Website: http://localhost/aa/websitelerim/
```

### CMS Sayfa Oluşturma
1. Admin panel → CMS → Yeni Sayfa
2. Hedef klasörü seçin (websitem/websitelerim)
3. Sayfa içeriğini TinyMCE ile düzenleyin
4. Kaydet → Otomatik PHP dosyası oluşturulur

### Araç Ekleme
1. Admin panel → Araçlar → Yeni Araç
2. Araç kategorisini seçin
3. Fotoğrafları yükleyin
4. Fiyat ve özellik bilgilerini girin

## 🔧 Geliştirici Bilgileri

### Kod Yapısı

#### **PHP Functions** (`php/`)
- `functions/auth_functions.php`: Kimlik doğrulama
- `functions/page_functions.php`: Sayfa yönetimi
- `functions/vehicle_functions.php`: Araç işlemleri
- `functions/booking_functions.php`: Rezervasyon işlemleri

#### **Admin Modules** (`admin/`)
- `cms_*.php`: CMS yönetim modülleri
- `dashboard.php`: Ana dashboard
- `vehicles.php`: Araç yönetimi
- `bookings.php`: Rezervasyon yönetimi

#### **Frontend Templates** (`websitem/`, `websitelerim/`)
- `includes/header.php`: Ortak header
- `includes/footer.php`: Ortak footer
- `*.php`: Sayfa şablonları

### API Endpoints
- **AJAX İşlemleri**: `/admin.php?action=`
- **Form Submits**: POST metodları
- **File Operations**: Dosya yükleme ve düzenleme

### JavaScript Modülleri
- **TinyMCE**: Zengin metin editörü
- **Bootstrap**: Responsive framework
- **jQuery**: DOM manipülasyonu

## 🧪 Test Dosyaları

Proje kapsamında çeşitli test dosyaları bulunmaktadır:

- `test_blog_system.php`: Blog sistemi testleri
- `test_complete_system.php`: Tam sistem testleri
- `test_menu_system.php`: Menü sistemi testleri
- `system_status_check.php`: Sistem durum kontrolü

## 📈 Proje Durumu

### ✅ Tamamlanan Özellikler
- Multi-website CMS sistemi
- Admin panel dashboard
- Araç yönetimi sistemi
- Rezervasyon sistemi
- Blog yönetimi
- İletişim form sistemi
- Multi-folder sayfa yönetimi
- TinyMCE entegrasyonu

### 🔄 Devam Eden Geliştirmeler
- SEO optimizasyonları
- Performans iyileştirmeleri
- Mobil uygulama API'si
- Ödeme sistemi entegrasyonu

## 🤝 Katkıda Bulunma

Bu proje açık kaynaklıdır ve katkılara açıktır. Geliştirme için:

1. Projeyi fork edin
2. Feature branch oluşturun
3. Değişikliklerinizi commit edin
4. Pull request gönderin

## 📧 İletişim

Proje hakkında sorularınız için:
- **E-mail**: atakan0909xxnxx@gmail.com
- **GitHub**: Proje repository'si
- **Dokümantasyon**: Bu README dosyası

## 📝 Lisans

Bu proje MIT lisansı altında yayınlanmıştır. Detaylı bilgi için LICENSE dosyasını inceleyiniz.

---

**Son Güncelleme**: Şubat 2026  
**Versiyon**: 2.1.0    
