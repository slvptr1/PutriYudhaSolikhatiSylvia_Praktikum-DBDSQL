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

- Membuat database akademik

![Create Database Akademik](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(303).png)

- Menggunakan database akademik

![Menggunakan Database Akademik](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(304).png)

📌 **Pembuatan database akademik dan menggunakannya dengan**
>create database AKADEMIK;
use akademik;

##### B. Membuat Table Strata, Seleksi_Masuk, Fakultas, Jurusan, Program_Studi, dan Mahasiswa #####
![Pembuatan Table Strata](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(305).png)
![Pembuatan Table Seleksi Masuk](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(306).png)
![Pembuatan Table Fakultas](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(307).png)
![Pembuatan Table Jurusan](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(308).png)
![Pembuatan Table Program Studi](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(309).png)
![Pembuatan Table Mahasiswa](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(310).png)

📌 **Cara yang digunakan untuk pengimplementasian syntax CREATE pada semua table yaitu dengan.**
> CREATE TABLE nama_tabel (
> kolom1 tipe_data1,
> kolom2 tipe_data2,
> kolom3 tipe_data3,
> PRIMARY KEY (kolom_utama)
>);

##### C. Insert data ke dalam Table #####
![Insert data ke dalam Fakultas](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(311).png)
![Insert data ke dalam Strata](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(312).png)
![Insert data ke dalam Jurusan](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(313).png)
![Insert data ke dalam Seleksi Masuk](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(314).png)
![Insert data ke dalam Program Studi](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(315).png)
![Insert data ke dalam Mahasiswa](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(316).png)

📌 **Cara yang digunakan untuk pengimplementasian syntax INSERT INTO pada table yaitu dengan.**
>INSERT INTO nama_table (kolom1, kolom2, kolom3, ...)
VALUES (nilai1, nilai2, nilai3, ...);

##### D. Mengambil Semua Data dari Table #####

 📌 **Cara yang digunakan untuk pengimplementasian syntax SELECT * FROM; pada semua table yaitu dengan.**
>SELECT * FROM nama_table;

##### 🤏 Implementasi Pada Soal Latihan 🤏 #####
![Select * From Mahasiswa;](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(246).png)
![Select * From Fakultas;](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(247).png)
![Select * From Jurusan](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(248).png)
![Select * From Program_Studi](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(249).png)
![Select * From Strata](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(250).png)


**Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/AKADEMIK.sql]
