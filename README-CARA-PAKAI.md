# ISTIQOMAH DATA — Panduan Aplikasi (Windows & Android)

**Istiqomah Data** adalah aplikasi **100% offline** untuk **Windows** dan **Android** yang mengolah file ekspor Excel data item dari **iPos 5** tanpa mengubah database asli iPos. Operasional kasir/penjualan toko tetap berjalan penuh di iPos.

## Fitur Utama
1. **Kontrol Laba & Margin Otomatis**: Memisahkan jenis **Level Harga (Ecer + Grosir)** dan **Satuan** serta multi-satuan (`pcs`, `pak`, `isi 3`, `isi 4`), lengkap dengan lampu indikator warna (merah / kuning / hijau) dan ekspor PDF / Excel.
2. **Order Supplier Otomatis (Excel Rapi Tanpa Harga)**: Mengelompokkan kebutuhan stok rendah/habis per prefix supplier (`ALMU`, `WRDA`, dll.), dilengkapi teks WhatsApp, PDF, dan **Ekspor Excel rapi tanpa harga** untuk langsung dikirim ke supplier.
3. **Deteksi Perubahan Harga Otomatis & Cetak Tag Harga Fleksibel**:
   - Setelah impor pertama, impor file ekspor Excel/CSV/SQL/JSON terbaru dari iPos langsung mendeteksi harga naik/turun, barang baru, dan stok rendah ke **Antrean Tag Harga**.
   - **Tag Harga Bersih**: Double border rapi menampilkan **Nama Produk**, **Harga Jual (`Rp.`)**, **Grosir kecil** (bila ada & berbeda dari harga ecer), dan **kode barcode teks saja** (tanpa gambar batang barcode agar ringkas ditempatkan di rak; item tanpa barcode tidak menampilkan kode item).
   - **Pilihan Kertas & Printer Fleksibel**: Mendukung **Thermal 58mm**, **Thermal 80mm**, **Kertas A4 Grid Multi-Kolom**, **Kertas A5**, **Kertas F4 / Folio**, **Stiker Label A4**, cetak langsung Printer Windows, ekspor PDF siap cetak, gambar PNG, ESC/POS Spooler/Serial/LAN, dan Bluetooth Android.
4. **Retur Barang per Supplier**: Pencatatan internal terpisah di SQLite lokal beserta laporan PDF / Excel.

---

## Cara Instalasi & Menjalankan
### Windows Desktop
1. **Installer Resmi (`Setup-IstiqomahData-v2.1.exe`)**: Jalankan installer dan ikuti langkah pemasangan. Pintasan muncul di Desktop & Start Menu dan berjalan langsung sebagai aplikasi Desktop native (tanpa jendela CMD).
2. **Portable Offline (`IstiqomahData-Portable-Windows.zip`)**: Ekstrak lalu jalankan `IstiqomahData.exe` di Windows 64-bit tanpa memerlukan internet atau instalasi .NET terpisah.

### Android
1. Unduh `IstiqomahData-Android.apk` lalu instal di HP/Tablet Android (Android 7.0+).
2. Mendukung cetak langsung ke printer thermal Bluetooth 58mm/80mm, printer LAN, maupun ekspor PDF/PNG untuk kertas A4/A5/F4.

- Database internal tersimpan lokal di `%LocalAppData%\IstiqomahData\istiqomah_data.db` (Windows) atau penyimpanan privat aplikasi (Android), serta dilengkapi **Backup & Restore** dan **Kunci PIN** di menu **Pengaturan**.

---
*made by Fahri Pratama*
