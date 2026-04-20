# CaptureFlow NW v1.2.10

- Tombol hapus riwayat capture sekarang benar-benar menghapus file lokal.
- Penghapusan capture sekarang ikut disinkronkan ke Nextcloud sebagai delete file spesifik.
- Hapus cloud dibuat aman untuk multi-device tanpa prune seluruh folder remote.

Perubahan utama:

- SAF delete sekarang fallback saat provider mengembalikan `false`.
- Metadata capture hanya dihapus setelah proses delete lokal tidak gagal.
- Sync queue mendapat tipe task khusus untuk delete file remote.
- Planner Nextcloud menormalisasi path file delete agar target remote tepat.

Catatan:

- Jika provider storage menolak operasi delete, app akan menampilkan error izin/folder yang lebih jelas.
