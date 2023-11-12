# MODUL 5 - Fungsi Skalar dan Fungsi Agregasi #

## 📅 Tanggal Praktikum ##
**7 November 2023**

##### Putri Yudha Solikhati Sylvia #####
##### 225150600111030 #####
---
## 📚 Apa itu _**"Fungsi Skalar"**_?
Fungsi skalar dalam SQL digunakan untuk mengembalikan nilai tunggal (single value)
dari suatu nilai input yang diberikan.

>> Beberapa jenis Fungsi Skalar : 
a. String Function : Concat(), Split_part(), Substr(), Length(), Replace(), Trim(), Upper(), Lower()
b. Numerik Function (Math) : Abs(), Ceiling(), Floor(), Round(), Sqrt(), Mod(), Exp()
c. Date Function : Curdate(), Curtime(), Timestamp()

## 📚 Apa itu _**"Fungsi Agregasi"**_?
Fungsi agregasi dalam SQL digunakan untuk melakukan perhitungan pada sekelompok nilai dan kemudian mengembalikan nilai tunggal.

>> Beberapa jenis Fungsi Agregasi : 
a. Sum()
b. Count()
c. Avg()
d. Min()
e. Max()
f. First()
g. Last()

## 🚀 Tugas Latihan
Coba semua fungsi yang ada pada Modul 5!

## 📸 Langkah Pengerjaan
Berikut adalah beberapa langkah-langkah beserta tangkapan layar pengerjaan tugas latihan:

**Percobaan Fungsi Skalar**
Data yang digunakan untuk mencoba fungsi skalar yaitu data yang ada pada database sampel_univeristy [https://raw.githubusercontent.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-BDSQL/main/sampel_university.sql]

1.  **Implementasi Semua Fungsi Skalar**
##### a. String Function #####
- Fungsi Concat
![Fungsi Concat](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(349).png)

Fungsi concat digunakan untuk menggabungkan semua argumen/input, NULL value akan diabaikan. Disini saya menggabungkan id dan nama dari table student. Kemudian menamainya dengan dataSiswa.

- Fungsi Substring_index
![Fungsi substring_index](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(351).png)

Fungsi substring_index digunakan untuk menampilkan string yang telah dipisah berdasarkan delimiter tertentu. 

- Fungsi Substr
![Fungsi substr](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(352).png)

Fungsi substr digunakan untuk menampilkan string berdasarkan string yang diinginkan. Disini saya menampilkan dept_name dengan mengambil 3 karakter dan dimulai dari huruf pertama.

- Fungsi Length
![Fungsi length](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(353).png)

Fungsi length digunakan untuk menghitung banyaknya karakter pada tiap data di suatu kolom. Disini saya menghitung banyaknya karakter dari data di kolom title.

- Fungsi Replace
![Replace](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(354).png)

Fungsi replace digunakan untuak menggantikan sebuah text dengan text yang diinginkan. Disini saya mengganti isi dari kolom semester yang awalnya Fall menjadi Winter. 

##### b. Numeric Function (Math) #####
- Fungsi Abs
![Fungsi Abs](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(355).png)

Fungsi abs atau absolute berfungsi untuk mengembalikan nilai absolute dari nilai input. Dikarenakan tidak ada nilai negatif dari data, maka saya mencoba fungsi ini dengan menggunakan data dari kolom start_hr table time_slot.

- Fungsi Ceiling
![Fungsi ceiling](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(357).png)

Fungsi ceiling digunakan untuk mengembalikan nilai integer terbesar dari nilai input. Disini saya menggunakan data dari kolom budget table department.

- Fungsi Floor
![Fungsi Floor](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(359).png)

Fungsi floor digunakan untuk mengembalikan nilai integer terkecil yang terdekat dari nilai input. Disini saya menggunakan data dari kolom start_hr table time_slot.

- Fungsi Round
![Fungsi Round](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(360).png)

Fungsi round digunakan untuk mengembalikan nilai pembulatan dari nilai desimal. Disini saya menggunakan data dari kolom budget table department.

- Fungsi Sqrt
![Fungsi sqrt](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(362).png)

Fungsi sqrt digunakan untuk mengembalikan nilai akar kuadrat dari nilai input. Disini saya menggunakan data dari kolom credits table course.

##### c. Date Function #####
- Fungsi Curdate
![Fungsi curdate](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(363).png)

Fungsi curdate digunakan untuk mengembalikan tanggal saat ini.

- Fungsi Curtime
![Fungsi curtime](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(364).png)

Fungsi curtime digunakan untuk mengembalikan waktu saat ini.

- Fungsi Tiemstamp
![Fungsi timestamp](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(365).png)

Fungsi timestamp digunakan unruk mengembalikan nilai datetime berdasarkan tanggal atau nilai datetime.

2.  **Implementasi Semua Fungsi Agregasi**
- Fungsi Sum
![Fungsi sum](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(366).png)

Fungsi sum digunakan untuk menjumlahkan sekelompok nilai(baris) dalam satu kolom. Disini saya menjumlahkan data pada kolom credits table course.

- Fungsi Count
![Fungsi count](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(367).png)

Fungsi count digunakan untuk menghitung jumlah baris. Disini saya menggunakan fungsi count untuk menghitung jumlah baris kolom credits table course.

- Fungsi Avg
![Fungsi avg](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(368).png)

Fungsi avg digunakan untuk menghitung rata-rata dari suatu kolom. Disini saya menggunakan fungsi avg untuk menghitung rata-rata dari kolom budget table department.

- Fungsi Min
![Fungsi min](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(369).png)

Fungsi min digunakan untuk menghitung nilai minimum dari suatu kolom. Disini saya menggunakan fungsi min untuk menghitung nilai minimum dari kolom credits table course.

- Fungsi Max
![Fungsi max](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(370).png)

Fungsi max merupakan kebalikan dari fungsi min. Disini saya gunakan fungsi max untuk menghitung nilai maximum dari kolom credits table course.

- Fungsi First
![Fungsi first](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(371).png)

Fungsi first digunakan untuk mengambil nilai pertama dari suatu kolom. Disini saya mengambil nilai pertama kolom name table instructor.

- Fungsi Last
![Fungsi last](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(372).png)

Fungsi last merupakan kebalikan dari fungsi first. Disini saya mengambil nilai terakhir kolom name table instructor.

- Fungsi Group By
![Group by](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(373).png)

Fungsi group by menggabungkan nilai yang sama ke dalam satu kolom. Disini saya menghitung dahulu id kemudian memasukkan jumlah masing masing ke dalam kolom semester (fall atau spring) kemudain menampilkannya.

- Fungsi Group By Having
![Group by having](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(374).png)

Fungsi group by having sama dengan group by akan tetapi menambah syarat untuk tampilan data dimana jika syarat terpenuhi maka data tersebut yang ditampilkan. Disini saya menambah syarat dimana apabila nilai dari count(id) bernilai > 50 maka data tersebut ditampilkan.

> **Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/sampel_university_modul5.sql]