# HAKIOS 1.0

HAKIOS adalah aplikasi simulasi antarmuka bergaya iOS untuk Android. Ini bukan iOS asli dan tidak menjalankan firmware Apple.

## Fitur demo
- Boot screen HAKIOS dan animasi loading
- Lock screen dengan jam/tanggal
- Home screen, ikon aplikasi, dan dock
- Control Center demo dengan tombol dan slider
- Settings demo
- Aplikasi demo: Photos, Camera, Calendar, Clock, Maps, Weather, Notes, Reminders, App Store, Health, Files, Phone, Safari, Messages, Music

## Build APK
1. Buka folder proyek ini di Android Studio.
2. Tunggu Gradle Sync selesai (butuh internet pertama kali untuk mengunduh Android Gradle Plugin).
3. Pilih **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. APK debug akan muncul di `app/build/outputs/apk/debug/app-debug.apk`.

## Catatan
- Target Android: API 35, minimum Android 6.0 (API 23).
- Tampilan dibuat dengan HTML/CSS/JavaScript di dalam WebView.
- Tombol Wi-Fi/Bluetooth/airplane mode hanya visual demo; aplikasi tidak mengubah pengaturan radio Android.
- Camera, Phone, Maps, Weather, App Store, Safari, dan layanan lain belum terhubung ke layanan asli.
- Gunakan nama/ikon sendiri jika ingin distribusi publik; logo Apple dan merek iOS adalah milik Apple.

## Build APK hanya dengan HP (tanpa Android Studio)
Proyek ini menyertakan GitHub Actions workflow di `.github/workflows/android.yml`.
1. Buat repository GitHub baru dari browser HP.
2. Upload seluruh isi folder proyek `HAKIOS` ke repository (termasuk folder `.github`).
3. Buka tab **Actions**, pilih **Build HAKIOS APK**, lalu tekan **Run workflow** jika belum berjalan otomatis.
4. Setelah workflow selesai hijau, buka hasil run dan unduh artifact **HAKIOS-debug-APK**.
5. Ekstrak artifact ZIP, lalu install `app-debug.apk` di HP.
Build dilakukan di server GitHub; HP hanya dipakai untuk mengunggah sumber dan mengunduh APK.
