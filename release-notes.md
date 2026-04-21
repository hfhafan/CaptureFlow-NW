# CaptureFlow NW v1.2.14

- Screenshot dibuat lebih responsif setelah izin sistem diberikan.
- Delay internal khusus screenshot dikurangi tanpa mengubah flow resmi MediaProjection.
- File target SAF dibuat setelah bitmap tercapture, jadi momen capture tidak menunggu operasi storage.

Perubahan utama:

- Delay setelah consent screenshot diturunkan dari 650 ms ke 180 ms.
- Delay settle screenshot di foreground service diturunkan dari 650 ms ke 160 ms.
- Wait resize MediaProjection Android 14+ diturunkan dari 450 ms ke 180 ms.
- Log timing debug ditambahkan untuk melihat durasi setiap tahap screenshot.

Catatan:

- Screenshot tetap tidak bisa secepat engine bawaan OS karena app biasa wajib memakai MediaProjection dan izin sistem.
