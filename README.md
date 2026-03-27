# 🏨 Otel Rezervasyon Sistemi (Java Console Application)

Bu proje, 100 oda kapasiteli bir otelin rezervasyon süreçlerini yönetmek için geliştirilmiş, dosya tabanlı saklama özelliğine sahip Java tabanlı bir otomasyon yazılımıdır.

## 🚀 Proje Hakkında
Java temel prensiplerini ve dosya yönetim sistemlerini uygulamak amacıyla geliştirilmiştir. Kullanıcı etkileşimli bir konsol menüsü üzerinden rezervasyon oluşturma, iptal etme, güncelleme ve arama fonksiyonlarını sunar.

## 🛠️ Teknik Özellikler & Uygulanan Kavramlar
Kod mimarisinde şu teknik yapılar kullanılmıştır:
* **Veri Yapıları:** Müşteri bilgileri ve oda durumlarını yönetmek için paralel diziler (`Arrays`) kullanıldı.
* **Method Overloading (Metot Aşırı Yükleme):** `rezervasyonAra()` metodu hem **Oda Numarası** hem de **TC Kimlik Numarası** ile arama yapabilecek şekilde iki farklı parametre yapısıyla (int ve long) optimize edildi.
* **Kalıcı Veri Yönetimi (File I/O):** `FileWriter` kullanılarak rezervasyon bilgileri `kayitlar.txt` dosyasına kalıcı olarak kaydedilir.
* **Sistem Geri Yükleme:** `sistemiYukle()` fonksiyonu ile uygulama her başlatıldığında, kayıtlı veriler dosyadan okunarak sistem otomatik olarak güncel duruma getirilir.
* **Dinamik Kontrol:** `boolean [] odaKontrol` dizisi ile odaların doluluk durumu anlık olarak takip edilir ve mükerrer kayıt engellenir.

## 📂 Menü Fonksiyonları
1. **Rezervasyon Oluştur:** Boş odaları listeleme ve müşteri bilgileriyle kayıt.
2. **Rezervasyon İptal:** Oda numarası üzerinden aktif rezervasyonu sonlandırma.
3. **Rezervasyon Güncelle:** Mevcut rezervasyon süresini uzatma ve ücret hesaplama.
4. **Rezervasyon Ara:** TC No veya Oda No ile müşteri bilgilerine hızlı erişim.
5. **Rezervasyonları Listele:** Dosyadaki tüm geçmiş kayıtları konsol ekranında görüntüleme.
