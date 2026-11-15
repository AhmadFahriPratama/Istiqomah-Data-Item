# PANDUAN SINGKAT — ISTIQOMAH DATA (v2.5.0)

Aplikasi operasional retail eksternal **100% Offline** untuk mendampingi **iPos** pada **Windows Desktop** (fokus penuh rilis Windows; pengembangan Android dijeda sementara).

## 1. Instalasi & Menjalankan di Windows
- **Menggunakan Installer (`Setup-IstiqomahData-v2.5.exe`)**:
  Klik 2x file `Setup-IstiqomahData-v2.5.exe`, ikuti langkah instalasi hingga selesai (tanpa memerlukan koneksi internet atau .NET tambahan), lalu buka **Istiqomah Data** dari shortcut Desktop atau Start Menu.
- **Menggunakan Paket Portable (`IstiqomahData-Portable-Windows.zip`)**:
  Ekstrak seluruh isi ZIP ke folder mana saja, lalu klik 2x **`IstiqomahData.exe`**.

## 2. Alur Operasional Harian (Pendamping iPos — 11 Modul Sidebar)
1. **Impor & Sync iPos (`ImportWizardView`)**:
   - Ekspor daftar item dari iPos ke file Excel (`.xlsx` / `.xls` / `.csv`) maupun `.sql` / `.json`.
   - Impor rutin menyediakan **Pratinjau & Validasi Pra-Simpan** (Terbaca, Baru, Diperbarui, Tidak Berubah, Bermasalah, Duplikasi, dan Tidak Ditemukan) dengan pilihan **Simpan Pembaruan** atau **Batalkan** sebelum mengubah database.
2. **Master Produk & Inspeksi Barcode (`MasterProdukView`)**:
   - Katalog terpaginasi (`25/50/100/200`), pencarian Kode/Barcode/Nama, filter Jenis & Supplier, panel detail varian/satuan/level 1–6+/supplier, serta deteksi **Konflik Barcode** (tanpa penggabungan otomatis).
3. **Arus Barang & Performa Produk (`ArusBarangView` & `ProductPerformanceView`)**:
   - Setiap sinkronisasi mempertahankan histori mutasi stok permanen (`stok_mutasi_log`) beserta status `TIDAK_DITEMUKAN_IMPOR` tanpa menyamakan pengurangan stok impor dengan penjualan kasir.
4. **Kontrol Laba (`ProfitControlView`)**:
   - Memisahkan perhitungan **Margin%** `(Harga Jual - Harga Beli) / Harga Jual` dan **Markup%** terhadap harga beli, dilengkapi guard harga beli invalid (`<= 0`), lampu status merah/kuning/hijau, dan rekomendasi harga pembulatan.
5. **Multi-Supplier & Order Supplier (`MultiSupplierView` & `OrderSupplierView`)**:
   - Mendukung **banyak supplier untuk satu produk** dengan perbandingan harga konversi per unit dasar (`HargaBeli / IsiPerSatuan`), pencatatan `supplier_price_history`, dan pemakaian `kode_item_supplier` milik supplier.
   - Format ekspor Excel Order ringkas dan bersih (tanpa harga, tanpa kolom TTD, tanpa kode item internal toko) dengan penamaan harian `Order_<Supplier>_YYYY-MM-DD-001.xlsx` (`-002`, `-003`, dst.).
6. **Pengaturan Level Harga 1–6+ & Cetak Tag Harga (`SettingsView` & `TagHargaView`)**:
   - Level Harga Ecer & Grosir dapat dikonfigurasi fleksibel (Level 1 s/d Level 6+) di **Pengaturan**, lengkap dengan validasi integritas **Backup & Restore SQLite**.
   - Tag Harga hanya menampilkan Nama Produk, Harga Jual (`Rp.`), Harga Grosir proporsional bila ada, dan Teks Kode Barcode (tanpa gambar garis barcode), mendukung A4, A5, F4, Stiker, dan Thermal 58mm/80mm.
7. **Retur Barang per Supplier (`ReturBarangView`)**:
   - Input banyak barang sekaligus untuk satu supplier dengan pencarian cepat, opsi pencatatan audit pengurangan stok terkonfirmasi `(RETUR_SUPPLIER)`, dan rekap nilai per periode.
