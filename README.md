# Istiqomah Data v2.4.0

Aplikasi **100% offline** untuk **Windows Desktop** dan **Android** guna mengolah ekspor data item Excel / CSV / SQL / JSON dari **iPos 5** tanpa mengubah database asli iPos.

## Fitur Utama
- **Dashboard Sederhana & Jujur**: Menampilkan status kesiapan operasional yang bersih tanpa grafik berlebihan dan menampilkan status **`Data Belum Tersedia`** secara jujur saat belum ada file Excel iPos yang diimpor.
- **Histori Perubahan Stok Permanen & Analisis Pergerakan Barang**: Mencatat riwayat perubahan stok (`stok_mutasi_log`) antar-impor secara permanen (tidak dihapus saat timpa penuh) dan menganalisis pergerakan barang secara jujur tanpa mengklaim selisih stok sebagai penjualan.
- **Multi-Supplier & Perbandingan Harga Supplier per Produk**: Mendukung banyak supplier untuk satu produk (`item_supplier_harga`), menandai supplier **`TERMURAH`**, menghitung selisih harga, dan terintegrasi langsung dengan penyusunan Order Supplier.
- **Sinkronisasi Penuh (Full Overwrite Catalog)**: Menimpa data katalog lama dengan file ekspor iPos terbaru secara menyeluruh sambil menjaga histori stok, riwayat cetak, perubahan harga, multi-supplier, order, dan retur.
- **Kontrol Laba & Level Harga Fleksibel (Level 1 – Level 6+)**: Mendukung hingga **6+ level harga iPos** serta multi-satuan, dilengkapi indikator lampu merah/kuning/hijau, saran pembulatan harga jual, dan ekspor Excel / PDF.
- **Order Supplier Ringkas & Urutan Harian `-001 / -002`**: Format Excel & PDF supplier yang bersih (`No | Nama Barang | Qty | Satuan | Catatan`) — tanpa Kode Item internal, tanpa kolom harga, dan tanpa kolom TTD — serta penamaan file Excel diakhiri tanggal dan nomor urut harian (`-yyyy-MM-dd-001.xlsx`, `-002.xlsx`, dst.).
- **Retur Barang Massal Banyak Item per Supplier**: Pilih banyak barang supplier sekaligus (`Pilih Terfilter`, edit `Qty Retur`, `+ Tambah Terpilih`) ke Draft Surat Jalan Retur, plus pencarian riwayat & rekap supplier.
- **Studio Tag Harga Bersih & Fleksibel**: Menampilkan **Nama Produk**, **Harga Jual (`Rp.`)**, **Grosir kecil** (sesuai level pilihan), dan **kode barcode teks saja** (tanpa gambar batang barcode; item tanpa barcode tidak menampilkan kode item).
- **Printer & Kertas Lengkap**: Mendukung **Thermal 58mm**, **Thermal 80mm**, **Kertas A4 Grid**, **Kertas A5 Grid**, **Kertas F4 Grid**, **Stiker Label A4**, cetak langsung Printer Windows, ekspor PDF siap cetak, gambar PNG, ESC/POS, serta Bluetooth Android.

## Unduhan Resmi ([Releases v2.4.0](https://github.com/AhmadFahriPratama/Istiqomah-Data-Item/releases/tag/v2.4.0))
- **`Setup-IstiqomahData-v2.4.exe`** — Installer resmi Windows 64-bit (bebas `Error Code 2`, Desktop & Start Menu).
- **`IstiqomahData-Portable-Windows.zip`** — Paket portabel Windows 64-bit self-contained.
- **`IstiqomahData-Android.apk`** — Paket instalasi Android (`Android 7.0+`).

Lihat [README-CARA-PAKAI.md](./README-CARA-PAKAI.md) untuk panduan penggunaan lengkap.

---
*made by Fahri Pratama*
