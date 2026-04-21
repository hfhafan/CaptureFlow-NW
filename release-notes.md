# CaptureFlow NW v1.2.13

- Auto-sync background dipastikan tetap aktif setelah Paksa Sinkron Sekarang selesai.
- Jika masih ada task sync yang pending setelah worker background dibatalkan sementara, app akan menjadwalkan ulang auto-sync.
- Paksa Sinkron Sekarang tetap berjalan langsung dan cepat dengan transfer paralel terbatas.

Perubahan utama:

- WorkManager background sync tetap memakai constraint network dan baterai.
- Force sync tidak menghapus atau mematikan antrean background untuk task lain.
- Query pending sync ditambahkan agar app bisa restore jadwal background sync dengan aman.

Catatan:

- Auto-sync background tetap hemat baterai; mode cepat hanya dipakai saat pengguna menekan Paksa Sinkron Sekarang.
