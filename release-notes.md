# CaptureFlow NW v1.2.12

- Tombol sync proyek sekarang bernama Paksa Sinkron Sekarang.
- Paksa sinkron tidak lagi masuk antrean background, tetapi langsung berjalan saat tombol ditekan.
- Proses paksa sinkron membatalkan worker background yang sedang dijadwalkan, lalu upload dan hapus file cloud dengan transfer paralel terbatas.

Perubahan utama:

- Auto-sync background tetap hemat baterai dan memakai constraint baterai seperti sebelumnya.
- Paksa sinkron memakai mode performa tinggi karena dijalankan manual oleh pengguna.
- Sinkronisasi WebDAV diberi guard agar force sync dan auto-sync tidak berjalan bersamaan.

Catatan:

- Jika koneksi cloud lambat, durasi sinkron masih bergantung pada jaringan, ukuran file, dan respons Nextcloud.
