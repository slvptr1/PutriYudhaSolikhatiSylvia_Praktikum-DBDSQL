# PRAKTIKUM 3 - DML (Data Manipulation Language)

## 📅 Tanggal Praktikum
**24 Oktober 2023**

##### Putri Yudha Solikhati Sylvia #####
##### 225150600111030 #####
---
## 📚 Apa itu _**"DML"**_?
Data Manipulation Language atau sering disebut DML adalah bahasa komputer yang digunakan untuk mengubah dan mengambil data dalam database. Manipulasi ini dilakukan dengan memasukkan data ke dalam tabel database, mengambil data yang ada, kemudian menghapus data dari tabel yang ada, ataupun memodifikasi data yang ada.

![SQL Commands](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-24%20202500.png)

## 🚀 Tugas Latihan
Berikut adalah soal praktikum Modul 7 :
1. Perhatikan Gambar Berikut!
![Physical Data Model Schema Akademik](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-24%20202738.png)
2. Lakukan insert data ke dalam tabel-tabel yang telah dibuat di Modul 6 DDL (No. 5 di Studi Kasus Modul 6) sesuai dengan Gambar 6, menggunakan data seperti data yang disediakan
dibawah ini
![Insert Data 1](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-24%20202753.png)
![Insert Data 2](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-24%20202804.png)

## 📸 Langkah Pengerjaan

Berikut adalah beberapa langkah-langkah beserta tangkapan layar pengerjaan tugas latihan:
##### A. Membuat database baru dengan CREATE DATABASE AKADEMIK; kemudian USE AKADEMIK; #####
![Create + Use Database Akademik](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(242).png)

📌 **Pembuatan database akademik dengan**
>create database AKADEMIK;
use akademik;

##### 👾 Bedah Syntax 👾 #####
- CREATE DATABASE AKADEMIK;: Merupakan perintah SQL yang digunakan untuk membuat database baru dengan nama "AKADEMIK". Setelah perintah ini dijalankan, database dengan nama "AKADEMIK" akan dibuat dan siap digunakan. Ini adalah langkah pertama dalam pembuatan database.
- USE akademik;: Merupakan perintah yang digunakan untuk beralih ke penggunaan (use) database yang telah dibuat. Dengan perintah ini, database yang diatur akan digunakan dalam sesi SQL selanjutnya menjadi "AKADEMIK". Artinya, semua perintah SQL selanjutnya akan berlaku untuk database "AKADEMIK" hingga Anda mengganti penggunaan database lagi dengan perintah USE yang lain.

##### B. Membuat Table Strata, Seleksi_Masuk, Fakultas, Jurusan, Program_Studi, dan Mahasiswa #####
![Pembuatan Table Database](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(242).png)
![Pembuatan Table Database](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(243).png)

📌 **Cara yang digunakan untuk pengimplementasian syntax CREATE pada semua table yaitu dengan.**
> CREATE TABLE nama_tabel (
> kolom1 tipe_data1,
> kolom2 tipe_data2,
> kolom3 tipe_data3,
> PRIMARY KEY (kolom_utama)
>);

📢 Membuat table dalam SQL melibatkan beberapa langkah dasar: 📢
- Tentukan Nama Tabel: Pilih nama untuk tabel yang akan dibuat.
- Tentukan Kolom: Tentukan kolom-kolom yang akan ada di dalam tabel. Untuk setiap kolom, perlu menentukan tipe data yang akan disimpan (seperti VARCHAR, INT, DATE, dll.) dan apakah kolom tersebut dapat menerima nilai NULL atau tidak.
- Tentukan Kunci Primer (Primary Key): Pilih satu atau beberapa kolom yang akan menjadi kunci utama (primary key) yang unik untuk setiap baris dalam tabel. Digunakan untuk mengidentifikasi setiap baris secara unik.
- Aturan Unik (Constraints): Tambahkan aturan unik atau aturan lainnya ke dalam tabel, seperti kunci asing (foreign key) untuk menghubungkannya dengan tabel lain, dan aturan seperti batasan CHECK untuk memvalidasi data yang dimasukkan.

##### C. Insert data ke dalam Table #####
![Insert data](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(245).png)

📌 **Cara yang digunakan untuk pengimplementasian syntax INSERT INTO pada table yaitu dengan.**
>INSERT INTO nama_table (kolom1, kolom2, kolom3, ...)
VALUES (nilai1, nilai2, nilai3, ...);

##### 👾 Bedah Syntax 👾 #####
- INSERT INTO: Ini adalah perintah SQL yang digunakan untuk menyisipkan (insert) data baru ke dalam tabel.
- nama_tabel: Ini adalah nama tabel di mana Anda ingin memasukkan data baru.
- (kolom1, kolom2, kolom3, ...): Ini adalah daftar kolom-kolom di dalam tabel yang akan diisi dengan nilai. Anda hanya perlu mencantumkan kolom-kolom yang ingin Anda isi dengan data baru.
- VALUES (nilai1, nilai2, nilai3, ...): Ini adalah daftar nilai yang akan dimasukkan ke dalam kolom-kolom yang telah disebutkan sebelumnya. Nilai-nilai ini harus sesuai dengan tipe data dan urutan kolom yang dijelaskan dalam perintah INSERT INTO.

##### D. Mengambil Semua Data dari Table #####
![Mengambil Data](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(246).png)
 
 📌 **Cara yang digunakan untuk pengimplementasian syntax SELECT * FROM; pada semua table yaitu dengan.**
>SELECT * FROM nama_table;

##### 👾 Bedah Syntax 👾 #####
- SELECT *: Merupakan perintah SQL yang digunakan untuk memilih (select) data dari table. Tanda asterisk (*) digunakan untuk menunjukkan bahwa semua kolom pada table akan diambil.
- FROM nama_table: Merupakan klausa yang digunakan untuk menunjukkan table yang ingin diambil datanya. 

##### 🤏 Implementasi Pada Soal Latihan 🤏 #####
![Select * From Mahasiswa;](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(246).png)
![Select * From Fakultas;](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(247).png)
![Select * From Jurusan](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(248).png)
![Select * From Program_Studi](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(249).png)
![Select * From Strata](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(250).png)


**Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/AKADEMIK.sql]