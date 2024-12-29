# Analisis Data Penjualan

## Deskripsi Tabel

### Tabel 1: Data Penjualan Bulanan
Tabel ini mencatat data penjualan bulanan untuk berbagai outlet, dengan struktur kolom sebagai berikut:
- **Branch**: Nama cabang tempat data penjualan berasal.
- **Cust ID**: ID pelanggan unik untuk setiap outlet.
- **Type Outlet**: Jenis outlet tempat transaksi dilakukan.
- **Jan-14** hingga **Jun-14**: Kolom yang mencatat jumlah penjualan untuk masing-masing bulan.

### Tabel 2: Mapping Type Outlet
Tabel ini digunakan untuk melakukan pemetaan jenis outlet berdasarkan kolom **Type**. Struktur tabel:
- **Type**: Jenis outlet.
- **Mapping**: Kategori yang terkait dengan jenis outlet tersebut.

### Tabel 3: Outlet Terpilih
Tabel ini berisi daftar outlet yang hanya mencatat beberapa **Kode Outlet** dan **Nama Outlet**. Tabel ini akan digunakan untuk menghubungkan outlet dengan data penjualan yang sudah ada di Tabel 1

---

## Tujuan Analisis

### **Tujuan 1: Menambahkan Kolom Mapping ke Tabel 1**
Langkah pertama dalam analisis ini adalah menambahkan informasi mengenai kategori outlet ke dalam **Tabel 1**. Dengan informasi ini, kita bisa mengetahui tipe outlet setiap cabang dan lebih mudah dalam memahami hasil penjualan yang ada.

### **Tujuan 2: Mengisi Tabel Baru Berdasarkan Data Penjualan**
Setelah menambahkan kolom **Mapping** di **Tabel 1**, langkah selanjutnya adalah mengisi **Tabel Baru** yang berisi outlet dan informasi penjualan untuk tiap bulan. Tabel ini akan diisi dengan data penjualan yang telah tercatat di **Tabel 1**, agar kita bisa mendapatkan gambaran lengkap mengenai kinerja outlet di setiap bulan yang tersedia.

### Tujuan 3: Melakukan Analisis Total Penjualan Berdasarkan Mapping
Langkah terakhir dalam analisis ini adalah menjumlahkan total penjualan untuk setiap kategori Mapping yang ada di Tabel 1.

## Disclaimer
Perlu dicatat bahwa data yang digunakan dalam analisis ini telah dibatasi.
