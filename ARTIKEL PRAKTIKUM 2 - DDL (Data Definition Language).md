# PRAKTIKUM 2 - DDL (Data Definition Language)

## 📅 Tanggal Praktikum
**17 Oktober 2023**

##### Putri Yudha Solikhati Sylvia #####
##### 225150600111030 #####
---
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
1. **Membuat skema dengan nama PENJUALANDVD**
![Skema PENJUALANDVD](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(239).png)

Cara yang dapat digunakan untuk membuat skema dengan nama PENJUALANDVD bisa dengan query **CREATE SCHEMA PENJUALANDVD** atau bisa juga dengan klik kanan pada database dan pilih **CREATE NEW DATABASE**. 
Apabila skema sudah dibuat, jalankan dan lihat output yang dikeluarkan. Untuk menggunakan database, gunakan query **use nama_schema**. Blok baris yang didalamnya terdapat query use PENJUALANDVD, kemudian jalankan.

2.  **Implementasi syntax CREATE pada semua table**
![CREATE Table Kecamatan](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(324).png)
![CREATE Table Movie ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(325).png)
![CREATE Table Genre ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(326).png)
![CREATE Table Kelurahan ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(327).png)
![CREATE Table Genre_Movie ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(328).png)
![CREATE Table Pelanggan ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(329).png)
![CREATE Table Kontak Pelanggan ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(330).png)
![CREATE Table Transaksi ](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(331).png)

📌 Cara yang digunakan untuk pengimplementasian syntax CREATE pada semua table yaitu dengan.
>**CREATE TABLE** nama_tabel (
> kolom1 tipe_data1,
> kolom2 tipe_data2,
> kolom3 tipe_data3,
> PRIMARY KEY (kolom_utama)
>);

**Pengecekan table PELANGGAN kolom JENIS_KELAMIN beri Check antara 'P' dan 'L'**

![Pengecekan Table PELANGGAN Kolom JENIS_KELAMIN](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(240).png)

📌 Pengecekan dilakukan dengan menggunakan ALTER TABLE
> ALTER TABLE pelanggan
 ADD CONSTRAINT jenis_kelamin_check CHECK (JENIS_KELAMIN IN ('P', 'L'));
 
 ✨ Berikut penjelasan mengenai syntax tersebut.
 
 Syntax tersebut adalah perintah SQL yang digunakan untuk menambahkan sebuah batasan (constraint) jenis kelamin pada kolom JENIS_KELAMIN dalam tabel pelanggan. Constraint ini memastikan bahwa nilai yang dimasukkan ke dalam kolom JENIS_KELAMIN hanya boleh 'P' atau 'L', yang mengindikasikan jenis kelamin "Perempuan" atau "Laki-laki".

3. Implementasi syntax **ALTER** untuk table **MOVIE** dengan **merubah tipe data kolom TAHUN_RILIS menjadi tipe data YEAR(4)**
![Perubahan Tipe Data Kolom TAHUN_RILIS menjadi Tipe Data YEAR(4)](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(240).png)

📌 Cara yang digunakan untuk merubah tipe data kolom TAHUN_RILIS menjadi YEAR yaitu dengan.
>  ALTER TABLE movie 
 MODIFY COLUMN tahun_rilis year;
 
✨ Berikut adalah penjelasan dari syntax tersebut:
 Syntax tersebut adalah perintah SQL yang digunakan untuk mengubah tipe data kolom tahun_rilis dalam tabel movie menjadi YEAR. Ini mengubah tipe data kolom tersebut sehingga hanya akan menerima tahun sebagai nilai (misalnya, 2023) dan akan membatasi jenis data yang dapat dimasukkan ke dalam kolom tersebut.

> **Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/PENJUALANDVD.sql]
