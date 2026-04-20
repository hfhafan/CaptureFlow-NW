# CaptureFlow NW v1.2.9

- Screenshot dari overlay tidak lagi membawa CaptureFlow ke foreground sebelum consent sistem.
- Android 14+ memakai dialog sistem MediaProjection untuk pilihan seluruh layar atau 1 aplikasi.
- Stabilitas capture diperbaiki untuk mengurangi race condition dan leak resource.

Perubahan utama:

- `CaptureConsentActivity` dibuat lebih transparan, tanpa animasi, dan tidak muncul di recent apps.
- Dialog mode screenshot buatan app tidak dipakai agar user tidak melihat popup dua kali.
- Resize callback MediaProjection dibuat lebih aman dari resume ganda.
- Bitmap dan ToneGenerator dirilis lebih defensif setelah screenshot.

Catatan:

- Di Android < 14, pilihan 1 aplikasi belum tersedia dari API resmi Android, jadi capture tetap seluruh layar.
