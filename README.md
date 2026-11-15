# Istiqomah Data v2.3.0

Aplikasi **offline** untuk **Windows Desktop** dan **Android** guna mengolah ekspor data item Excel / CSV / SQL / JSON dari **iPos 5** tanpa mengubah database asli iPos.

## Fitur Utama
- **Redesign Clean Enterprise SaaS**: Tampilan bersih & efisien (`#2563EB` Primary, `#172B4D` Navy, `#F5F7FB` Background, `#FFFFFF` Card), font Inter, sidebar ramping, KPI seragam, tabel data rapat & terbaca jelas.
- **Loading Overlay Ringan & Mulus**: Animasi XAML compositor 60fps (`made by Fahri Pratama`) dengan perpindahan layar & query database di background thread.
- **Sinkronisasi Penuh (Full Overwrite Catalog)**: Menimpa data katalog lama dengan file ekspor iPos terbaru secara menyeluruh (membersihkan item/satuan usang) sambil menjaga riwayat cetak, perubahan harga, order, retur, dan aturan toko.
- **Kontrol Laba & Level Harga Fleksibel (Level 1 – Level 6+)**: Mendukung hingga **6+ level harga iPos** serta multi-satuan, dilengkapi indikator lampu merah/kuning/hijau, saran pembulatan harga jual, dan ekspor Excel / PDF.
- **Level Ecer & Grosir Tag Harga Dapat Diatur**: Pengguna dapat menentukan **Level Harga Ecer** (`Level 1–6`) dan **Level Harga Grosir** (`Nonaktif` atau `Level 2–6`) langsung dari menu **Pengaturan**.
- **Order Supplier Ringkas & Urutan Harian `-001 / -002`**: Format Excel & PDF supplier yang bersih (`No | Nama Barang | Qty | Satuan | Catatan`) — tanpa Kode Item internal, tanpa kolom harga, dan tanpa kolom TTD — serta penamaan file Excel diakhiri tanggal dan nomor urut harian (`-yyyy-MM-dd-001.xlsx`, `-002.xlsx`, dst.).
- **Retur Barang Massal Banyak Item per Supplier**: Pilih banyak barang supplier sekaligus (`Pilih Terfilter`, edit `Qty Retur`, `+ Tambah Terpilih`) ke Draft Surat Jalan Retur, plus pencarian riwayat & rekap supplier.
- **Studio Tag Harga Bersih & Fleksibel**: Menampilkan **Nama Produk**, **Harga Jual (`Rp.`)**, **Grosir kecil** (sesuai level pilihan), dan **kode barcode teks saja** (tanpa gambar batang barcode; item tanpa barcode tidak menampilkan kode item).
- **Printer & Kertas Lengkap**: Mendukung **Thermal 58mm**, **Thermal 80mm**, **Kertas A4 Grid**, **Kertas A5 Grid**, **Kertas F4 Grid**, **Stiker Label A4**, cetak langsung Printer Windows, ekspor PDF siap cetak, gambar PNG, ESC/POS, serta Bluetooth Android.

## Unduhan Resmi ([Releases v2.3.0](https://github.com/AhmadFahriPratama/Istiqomah-Data-Item/releases/tag/v2.3.0))
- **`Setup-IstiqomahData-v2.3.exe`** — Installer resmi Windows (Desktop & Start Menu, tanpa jendela CMD).
- **`IstiqomahData-Portable-Windows.zip`** — Paket portabel Windows 64-bit self-contained.
- **`IstiqomahData-Android.apk`** — Paket instalasi Android (`Android 7.0+`).

Lihat [README-CARA-PAKAI.md](./README-CARA-PAKAI.md) untuk panduan penggunaan lengkap.

---
*made by Fahri Pratama*
