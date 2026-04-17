# CaptureFlow NW v1.2.6

- Popup screenshot tambahan dari app dihapus.
- Tombol screenshot sekarang langsung membuka dialog sistem Android.
- Alur screenshot jadi lebih cepat karena user hanya memilih mode sekali.

Perubahan utama:

- Overlay langsung meneruskan screenshot ke dialog MediaProjection sistem.
- Scope screenshot default diubah ke `user choice`, supaya sistem menangani pilihan layar penuh atau 1 aplikasi.
- Fix stabilitas screenshot Android 15 dari rilis sebelumnya tetap dipertahankan.

Catatan:

- Untuk game, tetap pilih `1 aplikasi` di dialog sistem jika layar penuh tidak akurat di perangkat tertentu.
