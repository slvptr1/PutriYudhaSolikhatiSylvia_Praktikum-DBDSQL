# PRAKTIKUM 2 - DDL (Data Definition Language)

## 📅 Tanggal Praktikum
**13 Oktober 2023**

## 📚 Apa itu _**"DDL"**_?
DDL merupakan salah satu bentuk SQL atau Structure Query Language yang bisa digunakan untuk menciptakan atau membuat database, tabel, struktur tabel, merubah struktur database, menghapus tabel, menghapus database serta membuat relasi antar tabel. Oleh sebab itu, DDL ini mempunyai sejumlah perintah dasar yang terdiri atas Create, Alter serta Drop.

## 🚀 Tugas Latihan
Berikut adalah soal praktikum Modul 6 :
1. Buatlah skema dengan nama **PENJUALANDVD**!
2. Implementasikan syntax **CREATE** untuk semua table pada Gambar 1! [https://drive.google.com/file/d/1YWZH3d4zzMhPRg6CxBz_vOKnUade4BCr/view?usp=sharing]
**Untuk table PELANGGAN kolom JENIS_KELAMIN beri Check antara 'P' dan 'L'**!
3. Implementasikan syntax **ALTER** untuk table **MOVIE** dengan **merubah tipe data kolom TAHUN_RILIS menjadi tipe data YEAR(4)**!



## 📸 Langkah Pengerjaan
Berikut adalah beberapa langkah-langkah beserta tangkapan layar pengerjaan tugas latihan:
1. Membuat skema dengan nama PENJUALANDVD
![Skema PENJUALANDVD](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(239).png)
> Cara yang dapat digunakan untuk membuat skema dengan nama PENJUALANDVD bisa dengan query CREATE SCHEMA PENJUALANDVD atau bisa juga dengan klik kanan pada database dan pilih CREATE NEW DATABASE


Apabila skema sudah dibuat, jalankan dan lihat output yang dikeluarkan. Untuk menggunakan database, gunakan query use NAMA_SCHEMA. Blok baris yang didalamnya terdapat query use PENJUALANDVD, kemudian jalankan.

2. Implementasi syntax CREATE pada semua table
![CREATE pada table](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(239).png)

Cara yang digunakan untuk pengimplementasian syntax CREATE pada semua table yaitu dengan.
>CREATE TABLE nama_tabel (
  kolom1 tipe_data1,
  kolom2 tipe_data2,
  kolom3 tipe_data3,
  PRIMARY KEY (kolom_utama)
);

Membuat tabel dalam SQL melibatkan beberapa langkah dasar:
- Tentukan Nama Tabel: Pilih nama untuk tabel yang akan dibuat.
- Tentukan Kolom: Tentukan kolom-kolom yang akan ada di dalam tabel. Untuk setiap kolom, perlu menentukan tipe data yang akan disimpan (seperti VARCHAR, INT, DATE, dll.) dan apakah kolom tersebut dapat menerima nilai NULL atau tidak.
- Tentukan Kunci Primer (Primary Key): Pilih satu atau beberapa kolom yang akan menjadi kunci utama (primary key) yang unik untuk setiap baris dalam tabel. Digunakan untuk mengidentifikasi setiap baris secara unik.
- Aturan Unik (Constraints): Tambahkan aturan unik atau aturan lainnya ke dalam tabel, seperti kunci asing (foreign key) untuk menghubungkannya dengan tabel lain, dan aturan seperti batasan CHECK untuk memvalidasi data yang dimasukkan.


