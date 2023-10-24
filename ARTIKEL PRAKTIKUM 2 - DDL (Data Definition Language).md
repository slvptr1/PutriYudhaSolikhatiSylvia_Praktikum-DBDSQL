# PRAKTIKUM 2 - DDL (Data Definition Language)

## 📅 Tanggal Praktikum
**13 Oktober 2023**

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
![CREATE pada table](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(239).png)

📌 Cara yang digunakan untuk pengimplementasian syntax CREATE pada semua table yaitu dengan.
>**CREATE TABLE** nama_tabel (
  kolom1 tipe_data1,
  kolom2 tipe_data2,
  kolom3 tipe_data3,
  PRIMARY KEY (kolom_utama)
);

📢 Membuat tabel dalam SQL melibatkan beberapa langkah dasar: 📢
- Tentukan Nama Tabel: Pilih nama untuk tabel yang akan dibuat.
- Tentukan Kolom: Tentukan kolom-kolom yang akan ada di dalam tabel. Untuk setiap kolom, perlu menentukan tipe data yang akan disimpan (seperti VARCHAR, INT, DATE, dll.) dan apakah kolom tersebut dapat menerima nilai NULL atau tidak.
- Tentukan Kunci Primer (Primary Key): Pilih satu atau beberapa kolom yang akan menjadi kunci utama (primary key) yang unik untuk setiap baris dalam tabel. Digunakan untuk mengidentifikasi setiap baris secara unik.
- Aturan Unik (Constraints): Tambahkan aturan unik atau aturan lainnya ke dalam tabel, seperti kunci asing (foreign key) untuk menghubungkannya dengan tabel lain, dan aturan seperti batasan CHECK untuk memvalidasi data yang dimasukkan.

**Pengecekan table PELANGGAN kolom JENIS_KELAMIN beri Check antara 'P' dan 'L'**

![Pengecekan Table PELANGGAN Kolom JENIS_KELAMIN](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(240).png)

📌 Pengecekan dilakukan dengan menggunakan ALTER TABLE
> ALTER TABLE pelanggan
 ADD CONSTRAINT jenis_kelamin_check CHECK (JENIS_KELAMIN IN ('P', 'L'));
 
 ✨ Berikut penjelasan mengenai syntax tersebut.
 
 Syntax tersebut adalah perintah SQL yang digunakan untuk menambahkan sebuah batasan (constraint) jenis kelamin pada kolom JENIS_KELAMIN dalam tabel pelanggan. Constraint ini memastikan bahwa nilai yang dimasukkan ke dalam kolom JENIS_KELAMIN hanya boleh 'P' atau 'L', yang mengindikasikan jenis kelamin "Perempuan" atau "Laki-laki".

### 👾 Bedah Syntax 👾 ###

- ALTER TABLE pelanggan: Merupakan perintah yang memberi tahu SQL bahwa akan dilakukan perubahan pada tabel pelanggan.
- ADD CONSTRAINT jenis_kelamin_check: Merupakan perintah yang menambahkan constraint baru ke tabel. Constraint ini dinamakan jenis_kelamin_check.
- CHECK (JENIS_KELAMIN IN ('P', 'L')): Menentukan aturan bahwa kolom JENIS_KELAMIN hanya boleh memiliki nilai 'P' atau 'L'. Jika dimasukkan nilai lain selain 'P' atau 'L' ke kolom JENIS_KELAMIN, maka akan terjadi kesalahan.

3. Implementasi syntax **ALTER** untuk table **MOVIE** dengan **merubah tipe data kolom TAHUN_RILIS menjadi tipe data YEAR(4)**
![Perubahan Tipe Data Kolom TAHUN_RILIS menjadi Tipe Data YEAR(4)](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(240).png)

📌 Cara yang digunakan untuk merubah tipe data kolom TAHUN_RILIS menjadi YEAR yaitu dengan.
>  ALTER TABLE movie 
 MODIFY COLUMN tahun_rilis year;
 
✨ Berikut adalah penjelasan dari syntax tersebut:

 Syntax tersebut adalah perintah SQL yang digunakan untuk mengubah tipe data kolom tahun_rilis dalam tabel movie menjadi YEAR. Ini mengubah tipe data kolom tersebut sehingga hanya akan menerima tahun sebagai nilai (misalnya, 2023) dan akan membatasi jenis data yang dapat dimasukkan ke dalam kolom tersebut.

### 👾 Bedah Syntax 👾 ###
- ALTER TABLE movie: merupakan perintah yang memberi tahu SQL bahwa akan dibuat perubahan pada tabel movie.
- MODIFY COLUMN tahun_rilis year: merupakan perintah yang memberi tahu SQL akan ada pengubahan kolom tahun_rilis. Dengan kata lain, sedang dilakukan modifikasi pada kolom tersebut.
- year: Merupakan perintah yang menentukan tipe data baru yang akan digunakan untuk kolom tahun_rilis. Dalam hal ini, tipe data yang ditentukan adalah YEAR. Dengan mengubah tipe data menjadi YEAR, kolom tahun_rilis hanya akan menerima tahun sebagai nilai (misalnya, 2023) dan akan membatasi jenis data yang dapat dimasukkan ke dalam kolom tersebut.

> **Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/PENJUALANDVD.sql]















 



