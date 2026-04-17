# CaptureFlow NW v1.2.5

- Crash screenshot Android 15 yang sempat memicu force close sudah diperbaiki.
- Mode screenshot sekarang lebih jelas: `Seluruh layar (standar)` dan `1 aplikasi (untuk game)`.
- Penanganan area capture dirapikan agar lebih stabil saat ukuran konten tangkap berubah.

Perubahan utama:

- Race condition callback `ImageReader` yang bisa memicu `Already resumed` sudah ditutup.
- Jalur MediaProjection diperbarui agar resize hasil tangkap ikut menyesuaikan area konten aktual.
- Overlay sekarang memberi petunjuk lebih jelas kapan sebaiknya memilih `1 aplikasi`.

Catatan:

- Pada sebagian Android 15 atau ROM tertentu, dialog sistem masih bisa menampilkan pilihan `1 aplikasi` sebagai default. Untuk game, gunakan mode `1 aplikasi`.
