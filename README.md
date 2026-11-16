# SonyOS Pro — OTA Güncelleme Deposu (updates/dist)

Bu depo, **SonyOS Pro** işletim sistemindeki yerleşik `sonyos_shell.dll` (`SonyOSUpdateAgent`) tarafından otomatik OTA güncelleştirmeleri ve toplu yamalar (`KB*`) için kullanılır.

## İçerik
- `sonyos-manifest.json` — Güncel sürüm, Build, KB numarası, indirme bağlantısı ve SHA-256 doğrulama özeti
- `SonyOS_Update_v*.zip` — İmzalı/SHA-256 doğrulanmış güncelleme arşivi (`install-update.ps1` veya `.msu` paketi içerir)

## Yayınlama Akışı (Geliştirici)
1. Ana projede `SonyOS-UpdatePublisher.ps1` aracını çalıştırın.
2. **GitHub Raw Kök Adresi** alanına `https://raw.githubusercontent.com/<KULLANICI_ADIN>/<REPO_ADIN>/main` yazıp **📌 Bu Adresi ISO İçine Kaydet** düğmesine basın.
3. **📦 Güncelleme Paketini ve Manifest'i Oluştur** ile `.zip` ve `sonyos-manifest.json` dosyalarını üretin.
4. **🚀 Git ile GitHub'a Gönder** düğmesi ile `main` dalına gönderin.
