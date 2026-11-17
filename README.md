# Orhaniyespor Satranç Kulübü – UKD Hesaplama (Android)

Bu proje, UKD Hesaplama Programı'nı Android uygulaması (APK) olarak paketler.
Uygulama tamamen telefonda çalışır, internet gerektirmez; veriler telefonda saklanır.

## APK nasıl oluşur?
GitHub'a her gönderimde **Actions → APK Oluştur** iş akışı çalışır ve APK'yı
**Releases** bölümüne ekler. Elle başlatmak için: Actions → APK Oluştur → Run workflow.

## Bilgisayarda derlemek (isteğe bağlı)
Android Studio ile klasörü açın → Build → Build APK(s).

## Telefona kurulum
1. Releases sayfasından `UKD-Hesaplama-....apk` dosyasını telefona indirin.
2. Dosyaya dokunun. İlk seferde "Bilinmeyen kaynaklardan yüklemeye izin ver" isteyebilir; izin verin.
3. Uygulama "UKD Hesaplama" adıyla ana ekranda görünür.

## Kalıcı imza (isteğe bağlı)
Güncellemelerin eski sürümün üzerine kurulabilmesi için depo ayarlarında şu sırları ekleyin:
`UKD_KEYSTORE_B64` (keystore dosyasının base64 hali), `UKD_KEYSTORE_PASSWORD`, `UKD_KEY_ALIAS`.
Sır yoksa APK hata ayıklama anahtarıyla imzalanır; yeni sürümü kurmadan önce eskisini kaldırmanız gerekebilir.
