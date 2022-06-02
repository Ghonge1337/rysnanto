+++
date = 2022-06-01T17:00:00Z
description = "Belajar menggunakan query sql seperti membuat database menambah dan lain sebagainya di comman prompt"
image = "/uploads/screenshot_20220602-164556_peluncur_pixel.png"
title = "Dokumentasi Belajar query sql  #1"

+++
Disclaimer : Mohon maaf bila ada penulisan atau query yang salah karena saya juga baru belajar menggunakan query sql, sebelumnya saya menggunakan phpmyadmin nya xampp untuk membuat sebuah database.

## Login Ke Mysql

pertama sebelum kita melakukan query kita perlu login terlebih dahulu ke mysql. Teman-teman bisa nyalakan mysql nya dengan cara buka XAMPP lalu tekan start pada mysql dan apache nya kalau perlu.

Buka command Prompt atau cmd , pastikan sudah berada di Penyimpanan **C:\\** , jika belum jangan khawatir bisa ketikan

<pre class="prettyprint">

Cd \\

</pre>

maka otomatis akan masuk ke penyimpanan utama.

Setalah itu teman teman bisa akases ke folder **xampp/mysql/bin** dengan cara mengetikkan perintah berikut ini

<pre class="prettyprint">

Cd xampp/mysql/bin

</pre>

cd disini adalah perintah untuk berpindah/masuk ke folder atau penyimpanan.

Sekarang kita bisa mengetikkan perintah ini untuk login ke mysql nya.

<pre class="prettyprint">

Mysql -u root

</pre>

saya akan jelaskan untuk perintah diatas.

**Keterangan :**

1. **-u root** ini adalah untuk memasukkan username dari mysql kamu, kebetulan username mysql saya adalah root

Dari penjelasan untuk login ke mysql nampak nya sangat ribet ya? gimana untuk shortcut nya saya kasih tau... , begini shortcutnya bisa teman teman ketikkan di cmd untuk cara cepat login mysql.

<pre class="prettyprint">

 cd xampp/mysql/bin && mysql -u root

</pre>

Saya berharap dengan tutorial diatas teman teman bisa memahami nya, mohon maaf bila ada typo ya....

## Membuat Database

Oke sekarang kita akan memulai menulis query untuk membuat database baru, caranya cukup simple sebenernya. untuk membuat database baru tinggal mengetikkan query di bawah ini

<pre class="prettyprint">

 CREATE DATABASE nama_database;

</pre>

ya kita beri perintah create ( membuat ) database dan diakhiri dengan nama database yang kita inginkan. jangan lupa untuk menghakhiri query kita perlu tambahkan **titik koma** ( wajib ).

lalu jika kita sudah membuat database sekarang yang jadi pertanyaan gimana cara kita masuk ke database tersebut? oh mudah sekali kamu tinggal mengetikkan sebuah perintah ini.

<pre class="prettyprint">

Use nama_database;

</pre>

Oke Itu dia pembahasan kita kali ini , kita masih akan berlanjut tentang sql ini yaitu cara membuat table dan menambah data. namun itu materi kita selanjutnya. Saya sertakan juga vi_io untuk materi kali ini agar lebih m_udah di pahami. Sekian erima kasih :3

{{< youtube btkYzsu35Pk >}}