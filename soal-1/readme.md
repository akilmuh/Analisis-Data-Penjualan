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


| Type | Mapping   |
|------|-----------|
| #    | RETAILER  |
| 1    | RETAILER  |
| 10   | MTISUPER  |
| 11   | MTIMINI   |
| 12   | MTISUPER  |
| 13   | RETAILER  |
| 2    | RETAILER  |
| 3    | RETAILER  |
| 4    | RETAILER  |
| 5    | RETAILER  |
| 6    | RETAILER  |
| 8    | RETAILER  |
| 9    | MTISUPER  |
| A    | WHOLESALER|
| B    | WHOLESALER|
| C    | WHOLESALER|
| D    | WHOLESALER|
| E    | RETAILER  |
| F    | RETAILER  |
| G    | RETAILER  |
| H    | RETAILER  |
| I    | RETAILER  |
| J    | RETAILER  |
| K    | RETAILER  |
| L    | RETAILER  |
| M    | RETAILER  |
| N    | RETAILER  |
| O    | MTISUPER  |
| P    | MTIMINI   |
| Q    | MTISUPER  |
| R    | RETAILER  |
| S    | RETAILER  |
| T    | RETAILER  |
| U    | RETAILER  |
| V    | RETAILER  |
| W    | RETAILER  |
| X    | MTISUPER  |
| Y    | RETAILER  |
| Z    | RETAILER  |
---

## Langkah-Langkah Analisis

### 1. Menambahkan Kolom Mapping ke Tabel 1
Langkah pertama adalah menambahkan kolom baru bernama **Mapping** di Tabel 1. Kolom ini diisi dengan merujuk ke Tabel 2, di mana jenis outlet yang ada di Tabel 1 akan dicocokkan dengan kategori **Mapping** di Tabel 2.

### 2. Mengisi Tabel Baru Berdasarkan Tabel 1
Tabel Baru yang diberikan memiliki kolom **Kode Outlet**, **Nama Outlet**, dan kolom **Jan-14** hingga **Jun-14** yang kosong. Tugas kita adalah mengisi kolom bulan tersebut dengan nilai yang sesuai berdasarkan data yang ada di Tabel 1. 

Proses pengisian dilakukan dengan cara merujuk pada **Cust ID** di Tabel 1 yang dicocokkan dengan **Kode Outlet** di Tabel Baru. Fungsi yang digunakan adalah **SUMIF**, yang akan menjumlahkan penjualan untuk setiap outlet berdasarkan **Kode Outlet** yang ada di Tabel Baru.

### 3. Hasil yang Diharapkan
Setelah pengisian selesai, Tabel Baru akan terisi dengan jumlah penjualan bulanan untuk setiap outlet, yang memungkinkan analisis data penjualan per outlet secara lebih terperinci.

---

## Kesimpulan
Dengan menggunakan **VLOOKUP** untuk menambahkan kolom **Mapping** dan **SUMIF** untuk menghitung nilai bulanan, kita dapat mengisi Tabel Baru dengan informasi penjualan yang sesuai untuk setiap outlet. Proses ini menyederhanakan analisis data penjualan bulanan dan memberikan gambaran yang jelas tentang performa masing-masing outlet.
