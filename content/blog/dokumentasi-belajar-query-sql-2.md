+++
date = 2022-06-02T17:00:00Z
description = "Melanjutkan belajar bersama tentang membuat table dan menambah data dengan query"
draft = false
image = ""
title = "Dokumentasi Belajar query sql #2"

+++
**Disclaimer** : Kita disini belajar bersama tentang query sql , mohon untuk di koreksi bila mana ada kesalahan penulisan di kolom komentar. Pada materi kali ini juga di sediakan Vidio agar mudah di pahami dan di mengerti.

## Membuat table

Setelah kita berhasil untuk login ke dalam mysql dan membuat sebuah database. Sekarang kita akan membuat sebuah table di dalam database yang kita buat. Query yang di gunakan yaitu

``` 
create table nama_table(
    	colom1 tipedata,
        colom2 tipedata
);
```

Jadi perintah untuk membuat table adalaha menggunakan create table dan di ikuti dengan nama table yang ingin teman-teman buat, setelah nama table di ikuti dengan tutup kurung dan di dalam tutup kurung tersebut diisi dengan nama **colom** dan **tipe data** nya apa. Jangan lupa jika ingin membuat beberapa kolom di pisah menggunakan tanda koma ( **,** ). Contoh  implementasi :

```  create table user(
    	nisn int(16) primary key,
        username varchar(25),
        password varchar(25)
    );
```

Untuk tipe data teman-teman bisa belajar di webiste w3school saja, karena kalau saya jelasin disini terlalu banyak dan takutna salah penyampaian [https://www.w3schools.com/sql/sql_datatypes.asp](https://www.w3schools.com/sql/sql_datatypes.asp "https://www.w3schools.com/sql/sql_datatypes.asp")

## Mengahapus Table

Jika teman-teman berfikir cara menghapus table nya gimana ternyata sama saat kita menghapus database, query nya adalah sebagai berikut 

```  
  DROP TABLE nama_table
```

Maka secara  otomatis tabel yang teman-teman pilih akan terhapus beserta data yang ada di dalamnya.

## Alter Table

Bagaimana saat kita lupa atau kurang nih colom nya tapi sudah terlanjur membuat table nya? , bukan hanya sekedar menambah coloumn baru tapi kita juga bisa memodifikasi column , menghapus coloumn dan lain-lain. lalu bagaiamana query nya?

1.  Menambah Column

``` 
ALTER TABLE nama_table ADD column_baru tipedata;
```

2.  Menghapus Column

```
ALTER TABLE nama_table DROP nama_column;
```


4.  Memodif column

```
ALTER TABLE nama_table MODIFY COLUMN column_yang_mau_diedit tipedata;
```

Kita sudah di ujung artikel kali ini mengenai Belajar query sql #2 ,Kita dapat mendapatkan cara membuat table, menghpus table , memodify column dan lain sebagainya. Mohon maaf bila ada kesalahan penulisan karena saya manusia biasa. Sekian terimakasih
<<youtube bLMHHlDO6do >>
