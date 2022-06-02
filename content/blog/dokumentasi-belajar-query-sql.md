+++
date = 2022-06-01T17:00:00Z
description = "Belajar menggunakan query sql seperti membuat database menambah dan lain sebagainya di comman prompt"
draft = true
image = ""
title = "[ Dokumentasi ] Belajar query sql "

+++
Disclaimer : Mohon maaf bila ada penulisan atau query yang salah karena saya juga baru belajar menggunakan query sql, sebelumnya sama menggunakan phpmyadmin nya xampp untuk membuat sebuah database.

## Login Ke Mysql

pertama sebelum kita melakukan query kita perlu login terlebih dahulu ke mysql. Teman-teman bisa nyalakan mysql nya dengan cara buka XAMPP lalu tekan start pada mysql dan apache nya kalau perlu.

Buka command Prompt atau cmd , pastikan sudah berada di Penyimpanan **C:\\** , jika belum jangan khawatir bisa ketikan 

    cd \

maka otomatis akan masuk ke penyimpanan utama.

Setalah itu teman teman bisa akases ke folder **xampp/mysql/bin** dengan cara mengetikkan perintah berikut ini 

    cd xampp\mysql\bin

cd disini adalah perintah untuk berpindah/masuk ke folder atau penyimpanan. 

Sekarang kita bisa mengetikkan perintah ini untuk login ke mysql nya 

    mysql -u root

 saya akan jelaskan untuk perintah diatas. 

**Keterangan :**

1. **-u root** ini adalah untuk memasukkan username dari mysql kamu, kebetulan username mysql saya adalah root

Dari penjelasan untuk login ke mysql nampak nya sangat ribet ya? gimana untuk shortcut nya saya kasih tau... , begini shortcutnya bisa teman teman ketikkan di cmd untuk cara cepat login mysql.

    cd xampp\mysql\bin && mysql -u root