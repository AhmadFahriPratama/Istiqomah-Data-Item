# Istiqomah Data v2.5.0

Aplikasi operasional retail **100% offline** untuk **Windows Desktop** guna mengolah ekspor data item Excel / CSV / SQL / JSON dari **iPos 5** tanpa mengubah database asli iPos. *(Fokus penuh pada rilis Windows Desktop `win-x64`; target Android dijeda sementara).*

## Fitur Utama (11 Modul Sidebar Desktop)
- **Dashboard Ringkas & Jujur (`Dashboard`)**: Menampilkan 4 KPI utama, 1 grafik tren pergerakan stok antar impor, maksimal 5 aktivitas terbaru, pencarian cepat produk, dan status database lokal (`Data Belum Tersedia` saat belum ada impor).
- **Impor & Sync iPos dengan Preview Pra-Simpan (`Impor & Sync iPos`)**: Mendukung `.xlsx`, `.xls`, `.csv`, `.sql`, dan `.json`. Menyediakan ringkasan validasi sebelum menyimpan (*Terbaca, Baru, Diperbarui, Tidak Berubah, Bermasalah, Duplikasi, Tidak Ditemukan*) dengan tombol **Simpan Pembaruan** atau **Batalkan** tanpa merusak database, ditambah animasi loading VSync halus `in-out` *"made by Fahri Pratama"*.
- **Master Produk & Konflik Barcode (`Master Produk`)**: Katalog produk terpaginasi (`25/50/100/200`), filter Jenis & Supplier, panel detail varian/ukuran/warna/multi-satuan/level harga 1–6+/histori stok, serta inspeksi bentrok barcode tanpa penggabungan otomatis.
- **Arus Barang Permanen (`Arus Barang`)**: Jejak audit `stok_mutasi_log` di setiap sinkronisasi tanpa dihapus saat timpa penuh (`TIDAK_DITEMUKAN_IMPOR`, tanpa menyamakan penurunan stok dengan penjualan kasir), lengkap dengan filter tanggal dan ekspor Excel/PDF.
- **Product Performance (`Performa Produk`)**: Analisis perputaran barang antar-impor (*Perputaran Cepat, Sedang, Lambat*) terpisah dari Dashboard dengan label sumber data yang jujur.
- **Multi-Supplier & Perbandingan Harga Setara Unit (`Multi-Supplier`)**: Mendukung banyak supplier per produk (`item_supplier_harga`) dengan normalisasi harga per unit dasar (`HargaBeli / IsiPerSatuan`), pencatatan `supplier_price_history`, dan pengelolaan `kode_item_supplier`.
- **Kontrol Laba Akurat Margin% vs Markup% (`Kontrol Laba`)**: Memisahkan Margin terhadap Harga Jual dan Markup terhadap HPP, menandai harga beli `<= 0` tanpa persentase palsu, indikator lampu merah/kuning/hijau, dan rekomendasi pembulatan harga.
- **Order Supplier Ringkas & Urutan Harian `-001 / -002` (`Order Supplier`)**: Menyusun order dengan kode katalog milik supplier terpilih dan mengekspor Excel ringkas tanpa harga, tanpa kolom TTD, dan tanpa kode item internal (`-yyyy-MM-dd-001.xlsx`, `-002.xlsx`, dst.).
- **Studio Tag Harga Bersih (`Tag Harga`)**: Menampilkan Nama Produk, Harga Jual (`Rp.`), Harga Grosir proporsional sesuai konfigurasi Level 1–6+, dan teks kode barcode saja, mendukung A4, A5, F4, Stiker, dan Thermal 58mm/80mm.
- **Retur Barang Massal & Rekap (`Retur Barang`)**: Input banyak barang sekaligus untuk satu supplier dengan opsi audit pengurangan stok terkonfirmasi `(RETUR_SUPPLIER)`.
- **Pengaturan & Backup Tervalidasi (`Pengaturan`)**: Konfigurasi fleksibel Level Harga Ecer & Grosir (Level 1–6+), aturan jenis & prefix supplier, printer Windows, PIN, serta Backup/Restore SQLite bervalidasi integritas file.

## Unduhan Resmi ([Releases v2.5.0](https://github.com/AhmadFahriPratama/Istiqomah-Data-Item/releases/tag/v2.5.0))
- **`Setup-IstiqomahData-v2.5.exe`** — Installer resmi Windows 64-bit self-contained (bebas `Error Code 2`, membuat shortcut Desktop & Start Menu).
- **`IstiqomahData-Portable-Windows.zip`** — Paket portabel Windows 64-bit self-contained.

Lihat [README-CARA-PAKAI.md](./README-CARA-PAKAI.md) untuk panduan penggunaan lengkap.

---
*made by Fahri Pratama*
