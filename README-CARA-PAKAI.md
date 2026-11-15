# PANDUAN SINGKAT — ISTIQOMAH DATA (v2.4.0)

Aplikasi operasional retail eksternal **100% Offline** untuk mendampingi **iPos** pada **Windows Desktop** dan **Android**.

## 1. Instalasi & Menjalankan di Windows
- **Menggunakan Installer (`Setup-IstiqomahData-v2.4.exe`)**:
  Klik 2x file `Setup-IstiqomahData-v2.4.exe`, ikuti langkah instalasi hingga selesai (tanpa memerlukan koneksi internet atau .NET tambahan), lalu buka **Istiqomah Data** dari shortcut Desktop atau Start Menu.
- **Menggunakan Paket Portable (`IstiqomahData-Portable-Windows.zip`)**:
  Ekstrak seluruh isi ZIP ke folder mana saja, lalu klik 2x **`IstiqomahData.exe`**.

## 2. Instalasi di Android (`IstiqomahData-Android.apk`)
- Salin file **`IstiqomahData-Android.apk`** ke HP/Tablet Android (minimal Android 8.0 / API 26).
- Buka file APK tersebut, izinkan instalasi dari sumber lokal bila diminta, lalu jalankan aplikasi **Istiqomah Data**.

## 3. Alur Operasional Harian (Pendamping iPos)
1. **Impor Pertama Data iPos**:
   - Ekspor daftar item dari iPos ke file Excel (`.xlsx` / `.xls` / `.csv`).
   - Buka menu **Impor & Sinkron iPos**, pilih file Excel tersebut, atur jenis barang yang memakai Tag Harga, periksa prefix supplier, dan klik **Simpan**.
2. **Sinkronisasi Berkala (Timpa Penuh & Histori Stok Otomatis)**:
   - Setiap ada pembaruan harga/stok di iPos, cukup pilih file Excel terbaru. Sistem menimpa katalog lama secara bersih, mempertahankan histori perubahan harga & **histori perubahan stok (`stok_mutasi_log`)**, serta menganalisis pergerakan barang secara jujur tanpa mengklaim selisih stok sebagai penjualan.
3. **Pengaturan Level Harga Grosir Fleksibel (Level 1 s/d 6)**:
   - Di menu **Pengaturan**, Anda dapat memilih Level Harga Ecer dan Level Harga Grosir (Level 1 sampai Level 6) sesuai struktur harga di iPos toko Anda.
4. **Cetak Tag Harga Bersih**:
   - Hanya menampilkan **Nama Produk**, **Harga Jual (Rp.)**, **Harga Grosir (ukuran proporsional lebih kecil bila ada)**, dan **Teks Kode Barcode** (hanya jika produk memiliki kode barcode; kode item internal tidak ditampilkan pada tag).
   - Mendukung ukuran kertas Thermal 58mm/80mm, A4, F4/Folio, Letter, A5, Label Sticker, dan Kustom.
5. **Order Supplier, Multi-Supplier & Analisis Pergerakan Barang**:
   - Mendukung **banyak supplier untuk satu produk** dan **perbandingan harga beli antar-supplier** secara langsung.
   - Menampilkan **Histori Perubahan Stok & Analisis Pergerakan Barang** antar-impor secara jujur.
   - Format ekspor Excel ringkas dan bersih (tanpa harga, tanpa kolom TTD, tanpa kode item internal) dengan penamaan otomatis `Order_<Supplier>_YYYY-MM-DD-001.xlsx` (`-002`, `-003` untuk pemesanan berikutnya di hari yang sama).
6. **Retur Barang per Supplier**:
   - Input banyak barang sekaligus untuk satu supplier menggunakan pencarian cepat & pemilihan masal di halaman **Retur Barang**.
