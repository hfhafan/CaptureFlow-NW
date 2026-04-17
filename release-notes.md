# CaptureFlow NW v1.2.7

- Startup app sekarang lebih cepat.
- Sesi login memakai cache lokal lebih dulu, lalu validasi server jalan di background.
- Katalog DUID tidak lagi ikut memuat saat app baru dibuka.

Perubahan utama:

- Auth startup tidak lagi menunggu `fetchConfig()` dari server sebelum UI utama tampil.
- Session cached tetap bisa langsung membuka app, lalu config server disegarkan tanpa menahan layar.
- Fetch daftar DUID dipindah ke saat tab DUID benar-benar dibuka.

Catatan:

- Jika server login mengganti versi sesi, app tetap akan meminta login ulang setelah refresh background selesai.
