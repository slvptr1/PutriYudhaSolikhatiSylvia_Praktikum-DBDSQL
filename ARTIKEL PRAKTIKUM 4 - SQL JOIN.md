# PRAKTIKUM 4 - SQL JOIN 

## 📅 Tanggal Praktikum
**31 Oktober 2023**

##### Putri Yudha Solikhati Sylvia #####
##### 225150600111030 #####
---
## 📚 Apa itu _**"JOIN TABLE"**_?
Perintah SELECT secara sederhana pada SQL merupakan perintah untuk memilih satu atau
lebih kolom yang ada pada satu tabel. Namun, kesulitan akan meningkat ketika perintah SELECT menggunakan tabel sebanyak dua atau lebih tabel sebagai sumber data yang ingin ditampilkan. Hal ini membuat banyak kemungkinan mengenai hasil akhir yang di dapat. Sehingga, Join tabel digunakan untuk mengambil data dari beberapa tabel melalui sat query.

##### Berikut ini adalah tipe join pada SQL: #####

**1. Inner Join**
Digunakan untuk mengembalikan baris-baris dari dua tabel atau lebih yang memenuhi syarat yang dibuat.

###### Jenis - jenis Inner Join : ######
- Equi Join : digunakan ketika dua tabel digabungkan berdasarkan kesamaan kolom
yang telah ditentukan.
- Cross Join : penggabungan dari tabel menggunakan metode Cartesian Product sederhana, yakni menggabungkan setiap row dari tabel pertama dengan setiap row pada tabel kedua.
- Join On : operasi inner join pada dua tabel atau lebih. Pada operasi inner join
kita juga bisa menambahkan klausa WHERE.
- Menggabungkan Lebih dari 2 Tabel

**2. Outer Join**
Bentuk penggabungan khusus yang digunakan pada perintah SQL. Pada outer join, tabel pertama yang ditentukan pada perintah SQL pada klausa FROM, ditandai sebagai tabel KIRI dan tabel selain itu ditandai sebagai tabel KANAN.

###### 3 Tipe Outer Join ######
- Left Outer Join
![Left Outer Join](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-31%20185138.png)
>> Pada left outer join, hasil akhir merupakan dari hasil akhir equi join, sekaligus beberapa baris dari tabel KIRI yang tidak memiliki relasi dengan tabel KANAN.
- Right Outer Join
![Right Outer Join](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-31%20185153.png)
Pada right outer join, hasil akhir merupakan perpaduan dari hasil akhir equi join, termasuk beberapa baris dari tabel KANAN yang tidak memiliki relasi dengan tabel KIRI.
- Full Outer Join
![Full Outer Join](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%202023-10-31%20185207.png)
Pada full outer join, hasil akhir merupakan perpaduan (union) dari hasil akhir equi-join, termasuk beberapa baris dari tabel KANAN dan KIRI yang tidak cocok.

**3. Self Join**
Perpaduan dari hasil akhir equi join suatu tabe dengan tabel itu sendiri.

## 🚀 Tugas Latihan
Berikut adalah soal praktikum Modul 8 :

🤏Mengacu pada data berikut. [https://drive.google.com/drive/folders/1PP6tSH-XIAokt00jeOhxXxTc3rQ26Ra2?usp=sharing] 🤏

Silakan download dan jalankan, kemudian lakukan perintah soal berikut :
1. Tampilkan semua nama Mahasiswa beserta nama department.
2. Tampilkan semua nama student beserta nama department yang memiliki total SKS
(total credit) lebih dari 100.
3. Tampilkan nama student dan nama instructor yang bekerja pada department yang sama

## 📸 Langkah Pengerjaan

Berikut adalah beberapa langkah-langkah beserta tangkapan layar pengerjaan tugas latihan:
##### A. Membuat database baru dengan create database sampel_university; #####
![Create Database sampel_university](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(261).png)

📌 **Pembuatan database akademik dengan**
>create database sampel_university;

##### 👾 Bedah Syntax 👾 #####
- create database sampel_university;  
Merupakan perintah SQL yang digunakan untuk membuat database baru dengan nama "sampel_university". 

##### B. Menggunakan database sampel_university #####
![Menggunakan database sampel_university](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(262).png)

📌 **Cara yang digunakan untuk menggunakan database sampel_university dengan**
> use sampel_university;

##### 👾 Bedah Syntax 👾 #####
- USE akademik; 
Merupakan perintah yang digunakan untuk beralih ke penggunaan (use) database yang telah dibuat. Dengan perintah ini, database yang diatur akan digunakan dalam sesi SQL selanjutnya menjadi "sampel_akademik". 

##### C. Membuat table classroom, department, course, instructor, section, teaches, student, takes, advisor, time_slot, dan prereq #####

📢 Membuat table dalam SQL melibatkan beberapa langkah dasar: 📢
- Tentukan Nama Tabel: Pilih nama untuk tabel yang akan dibuat.
- Tentukan Kolom: Tentukan kolom-kolom yang akan ada di dalam tabel. Untuk setiap kolom, perlu menentukan tipe data yang akan disimpan (seperti VARCHAR, INT, DATE, dll.) dan apakah kolom tersebut dapat menerima nilai NULL atau tidak.
- Tentukan Kunci Primer (Primary Key): Pilih satu atau beberapa kolom yang akan menjadi kunci utama (primary key) yang unik untuk setiap baris dalam tabel. Digunakan untuk mengidentifikasi setiap baris secara unik.
- Aturan Unik (Constraints): Tambahkan aturan unik atau aturan lainnya ke dalam tabel, seperti kunci asing (foreign key) untuk menghubungkannya dengan tabel lain, dan aturan seperti batasan CHECK untuk memvalidasi data yang dimasukkan.

**Berikut beberapa table yang dibuat pada Modul 8**
1. Table classroom
![Table classroom](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(263).png)
2. Table department
![Table department](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(264).png)
3. Table course
![table course](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(265).png)
4. Table instructor
![table instructor](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(266).png)
5. Table section
![Table section](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(267).png)
6. Table teaches
![Table teaches](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(268).png)
7. Table student
![Table student](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(269).png)
8. Table takes
![Table takes](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(270).png)
9. Table advisor
![Table advisor](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(271).png)
10. Table time_slot
![Table time_slot](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(272).png)
11. Table prereq
![Table prereq](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(273).png)


##### D. Insert data ke dalam Table #####

📌 **Cara yang digunakan untuk pengimplementasian syntax INSERT INTO pada table yaitu dengan.**
>INSERT INTO nama_table (kolom1, kolom2, kolom3, ...)
VALUES (nilai1, nilai2, nilai3, ...);

**Berikut implementasi syntax insert into pada table pada Modul 8**
1. Insert into time_slot values
![Insert into time_slot values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(282).png)
2. Insert into classroom values
![Insert into classroom values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(283).png)
3. Insert into deaprtment values 
![Insert into department values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(284).png)
4. Insert into course values 
![Insert into course values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(285).png)
5. Insert into instructor values
![Insert into instructor values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(286).png)
6. Insert into section values 
![Insert into section values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(287).png)
7. Insert into teaches values
![Insert into teaches values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(288).png)
8. Insert into student values 
![Insert into student values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(289).png)
9. Insert into takes values 
![Insert into takes values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(290).png)
10. Insert into advisor values
![Insert into advisor values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(291).png)
11. Insert into prereq values
![Insert into prereq values](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(292).png)

##### 👾 Bedah Syntax 👾 #####
- INSERT INTO: Ini adalah perintah SQL yang digunakan untuk menyisipkan (insert) data baru ke dalam tabel.
- nama_tabel: Ini adalah nama tabel di mana Anda ingin memasukkan data baru.
- (kolom1, kolom2, kolom3, ...): Ini adalah daftar kolom-kolom di dalam tabel yang akan diisi dengan nilai. Anda hanya perlu mencantumkan kolom-kolom yang ingin Anda isi dengan data baru.
- VALUES (nilai1, nilai2, nilai3, ...): Ini adalah daftar nilai yang akan dimasukkan ke dalam kolom-kolom yang telah disebutkan sebelumnya. Nilai-nilai ini harus sesuai dengan tipe data dan urutan kolom yang dijelaskan dalam perintah INSERT INTO.

##### D. Menampilkan semua nama Mahasiswa beserta nama department #####
![Menampilkan semua nama Mahasiswa beserta nama department](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(276).png)
 
 📌 **Cara yang digunakan untuk menampilkan semua nama Mahasiswa beserta nama department.**
>SELECT s.name AS Nama_Mahasiswa, d.dept_name AS Department
FROM student s
LEFT JOIN department d ON s.dept_name = d.dept_name;

##### E. Menampilkan semua nama student beserta nama department yang memiliki total SKS (total credit) lebih dari 100 #####
![Menampilkan semua nama student beserta nama department yang memiliki total SKS (total credit) lebih dari 100](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(277).png)

 📌 **Cara yang digunakan untuk menampilkan semua nama student beserta nama department yang memiliki total SKS (total credit) lebih dari 100.**
>SELECT s.name AS Nama_Mahasiswa, d.dept_name AS Department
FROM student s
INNER JOIN department d ON s.dept_name = d.dept_name
WHERE s.tot_cred > 100;

##### F. Menampilkan nama student dan nama instructor yang bekerja pada department yang sama #####
![Menampilkan nama student dan nama instructor yang bekerja pada department yang sama](https://github.com/slvptr1/IniGambarPrakSQL/blob/main/Screenshot%20(278).png)

 📌 **Cara yang digunakan untuk menampilkan nama student dan nama instructor yang bekerja pada department yang sama**
>SELECT s.name AS student_name, i.name AS instructor_name
FROM student s
JOIN instructor i on s.dept_name = i.dept_name;

**Kode selengkapnya pada link berikut** [https://github.com/slvptr1/PutriYudhaSolikhatiSylvia_Praktikum-DBDSQL/blob/main/sampel_university.sql]