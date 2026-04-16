# CaptureFlow NW v1.2.4

- Header login dirapikan agar ikon brand tetap terbaca jelas di layar HP yang sempit.
- Kanal distribusi customer dipisah dari source repo agar update dibuka lewat browser.
- Metadata update disiapkan untuk mode wajib update di rilis berikutnya.
- Secret bootstrap GAS dibersihkan dari source tracked.

Perubahan utama:

- Modal editor template diatur ulang agar tetap besar, tapi tidak lagi turun ke area navbar.
- Tombol aksi bawah diaudit ulang langsung dari device ADB dan dipastikan naik aman dari gesture bar.
- Tab bawah sekarang selalu tampil, termasuk saat belum ada proyek aktif.
- Script debug diperbaiki agar APK debug bisa langsung diluncurkan lagi setelah install.

Catatan:

- Update ini wajib karena memperbaiki safe zone layout yang berisiko di layar Android tertentu.
