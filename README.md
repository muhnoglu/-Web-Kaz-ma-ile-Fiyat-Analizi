# Web Kazıma ile Rakip ve Fiyat Analizi

## 📚 Proje Tanıtımı

Bu proje, **online kitap satışı yapan bir şirketin** "Seyahat" ve "Kurgu Dışı" kategorilerindeki kitaplara ait verileri kazıyıp, **rakip ve fiyat analizi** yapmasını sağlamak amacıyla geliştirilmiştir. Proje, **[books.toscrape.com](https://books.toscrape.com/)** adresindeki bu kategorilerdeki kitapları kazıyarak, **fiyat, yorum, yıldız sayısı** gibi metrikler üzerinde keşifsel veri analizi gerçekleştirmektedir.

## 🎯 İş Problemi

Şirket, özellikle "Seyahat" ve "Kurgu Dışı" kategorilerinde düşük satış performansı gözlemlemiştir. Rakip firmaların fiyat stratejilerini analiz edebilmek ve kendi fiyatlandırmalarını optimize etmek için bu kategorilere ait verileri kazıyarak, **rekabetçi fiyat analizi** yapmak istemektedir. Bu proje, kitapların fiyatları, yıldız sayıları ve diğer veriler üzerinden **derinlemesine analizler** yapmayı hedeflemektedir.

## 🧑‍💻 Kullanılan Teknolojiler

- **Python 3.x**: Proje için Python programlama dili kullanılmıştır.
- **Selenium**: Web tarayıcısını kontrol etmek ve sayfaları kazımak için Selenium WebDriver kullanılmıştır.
- **BeautifulSoup**: HTML ve XML verilerini işlemek ve verileri çekmek için BeautifulSoup kütüphanesi kullanılmıştır.
- **Regex (Düzenli İfadeler)**: Özellikle kitapların yıldız sayısı gibi verilerin çekilmesinde düzenli ifadeler kullanılmıştır.
- **Pandas**: Verilerin analiz edilmesi ve işlenmesi için pandas kütüphanesi kullanılmıştır.

## 🔍 Proje Akışı

### 1. **Tarayıcı Konfigürasyonu ve Başlatma**
- Selenium kullanılarak **Chrome** tarayıcısı başlatılmış ve tam ekran modunda çalışacak şekilde konfigüre edilmiştir.

### 2. **Ana Sayfa İncelemesi ve Kazınması**
- **Ana sayfa** üzerinden "Seyahat" ve "Kurgu Dışı" kategorilerine ait sayfa linkleri kazınmıştır.

### 3. **Kategori Sayfasının İncelenmesi**
- İlgili kategorilerdeki kitapların **detay sayfa linkleri** kazınmıştır. 
- Sayfalandırma işlemi, sayfa URL'leri manipüle edilerek yapılmıştır.

### 4. **Ürün Detay Sayfasının Kazınması**
- Kitapların **detay sayfasından** kitap adı, fiyatı, yıldız sayısı, açıklama gibi bilgilerin kazınması sağlanmıştır.

### 5. **Fonksiyonlaştırma ve Sürecin Otomatize Edilmesi**
- Verilerin toplanması süreci **otomatikleştirilmiş ve fonksiyonlar** aracılığıyla modüler hale getirilmiştir.

## 📊 Keşifsel Veri Analizi

Projede yapılan analizler sonucunda şu bulgular elde edilmiştir:

- **Yıldız Sayısı ile Kitap Fiyatları Arasındaki Korelasyon**: **0.08**
  - Yıldız sayısının kitap fiyatlarıyla zayıf bir korelasyona sahip olduğu gözlemlenmiştir.
  - **Fiyat** ve **Yıldız Sayısı** arasında çok güçlü bir ilişki bulunmamaktadır, ancak bazı kategorilerde fiyatlar arttıkça yıldız sayısının da arttığı gözlemlenmiştir.


