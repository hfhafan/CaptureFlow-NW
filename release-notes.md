# CaptureFlow NW v1.2.8

- Clone proyek dari cloud sekarang lebih stabil dan progresnya lebih jelas.
- Buka proyek lokal yang sudah ada sekarang kembali normal.
- Sinkronisasi cloud diperbaiki agar merge lokal dan refresh dari cloud lebih aman.

Perubahan utama:

- Parser respons WebDAV diperkeras agar tidak gagal di device tertentu.
- Metadata proyek duplikat dibersihkan otomatis saat app mulai.
- Proses clone dan refresh lokal mengurangi traversal folder yang tidak perlu.
- Status sinkronisasi sekarang menampilkan progres, jadi tidak terasa hang.

Catatan:

- Waktu sinkronisasi tetap bergantung pada jumlah file dan respons server Nextcloud.
