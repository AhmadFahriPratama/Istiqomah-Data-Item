# ISTIQOMAH DATA — Panduan Aplikasi (Windows & Android)

**Istiqomah Data** adalah aplikasi **offline** untuk **Windows** dan **Android** yang mengolah file ekspor Excel/CSV/SQL/JSON data item dari **iPos 5** tanpa mengubah database asli iPos. Operasional kasir/penjualan toko tetap berjalan penuh di iPos.

## Fitur Utama
1. **Sinkronisasi Penuh (Full Overwrite Catalog)**: Setiap impor/sync menimpa data katalog aktif dengan ekspor iPos terbaru secara penuh (membersihkan item/satuan usang agar terhindar dari bug sisa data) sambil tetap menjaga riwayat cetak, riwayat perubahan harga, order, retur, dan aturan toko.
2. **Kontrol Laba & Level Harga Fleksibel (Level 1 – Level 6+)**: Mendukung hingga **6+ level harga iPos** serta **Satuan / multi-satuan** (`pcs`, `pak`, `isi 3`, `isi 4`), lengkap dengan lampu indikator warna (merah / kuning / hijau) dan ekspor PDF / Excel.
3. **Order Supplier Ringkas & Rapi**: Mengelompokkan kebutuhan stok rendah/habis per prefix supplier (`ALMU`, `WRDA`, dll.) dengan **Ekspor Excel/PDF ringkas** (`No | Nama Barang | Qty | Satuan | Catatan` — tanpa Kode Item internal, tanpa harga, dan tanpa kolom TTD) serta teks WhatsApp siap kirim.
4. **Cetak Tag Harga Bersih & Level Grosir Dapat Diatur**:
   - Pengguna dapat memilih **Level Harga Ecer** (`Level 1–6`) dan **Level Harga Grosir** (`Nonaktif` atau `Level 2–6`) di menu **Pengaturan**.
   - **Tag Harga Bersih**: Double border rapi menampilkan **Nama Produk**, **Harga Jual (`Rp.`)**, **Grosir kecil** (sesuai level pilihan, bila berbeda dari harga utama), dan **kode barcode teks saja** (tanpa gambar batang barcode; item tanpa barcode tidak menampilkan kode item).
   - **Pilihan Kertas & Printer Fleksibel**: Mendukung **Thermal 58mm**, **Thermal 80mm**, **Kertas A4 Grid Multi-Kolom**, **Kertas A5**, **Kertas F4 / Folio**, **Stiker Label A4**, cetak langsung Printer Windows, ekspor PDF siap cetak, gambar PNG, ESC/POS Spooler/Serial/LAN, dan Bluetooth Android.
5. **Retur Barang per Supplier**: Pencatatan internal terpisah di SQLite lokal beserta laporan PDF / Excel.

---

## Cara Instalasi & Menjalankan
### Windows Desktop
1. **Installer Resmi (`Setup-IstiqomahData-v2.2.exe`)**: Jalankan installer dan ikuti langkah pemasangan. Pintasan muncul di Desktop & Start Menu dan berjalan langsung sebagai aplikasi Desktop native (tanpa jendela CMD).
2. **Portable Offline (`IstiqomahData-Portable-Windows.zip`)**: Ekstrak lalu jalankan `IstiqomahData.exe` di Windows 64-bit tanpa memerlukan internet atau instalasi .NET terpisah.

### Android
1. Unduh `IstiqomahData-Android.apk` lalu instal di HP/Tablet Android (Android 7.0+).
2. Mendukung cetak langsung ke printer thermal Bluetooth 58mm/80mm, printer LAN, maupun ekspor PDF/PNG untuk kertas A4/A5/F4.

- Database internal tersimpan lokal di `%LocalAppData%\IstiqomahData\istiqomah_data.db` (Windows) atau penyimpanan privat aplikasi (Android), serta dilengkapi **Backup & Restore** dan **Kunci PIN** di menu **Pengaturan**.

---
*made by Fahri Pratama*
