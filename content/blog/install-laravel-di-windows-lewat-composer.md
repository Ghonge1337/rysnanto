---
title: Begini Cara Install Laravel Di Windows Menggunakan Composer
date: 2016-06-1
description: Laravel yang akan kita install semua di handle oleh Composer
image: images/pos1laravelthumb.png
draft: false
---

Bagaimana Cara install laravel lewat composer? , berikut ini adalah sebuah tutorial dari saya
yang baru menggunakan / mempelajari laravel. ada 2 cara sebenernya untuk menginstall framework php ini, kita fokus install laravel menggunakan bantuan Composer. Sebelumnya apa itu composer? Composer tools dependency manager pada PHP atau biasa di gunakan untuk mengunduh library yang tersedia di packgist. jadi semua yang kita butuhkan untuk bergelud dengan bahasa php ada di composer secara otomatis.

Lalu sekarang bagaimana cara install laravel lewat composer? Caranya mudah teman.Teman-teman bisa mengunduh aplikasi composer di website resmi nya atau klick unduh untuk mendownload aplikasi composer nya. Teman-teman juga harus memastikan di dalam komputer teman teman terdapat xampp yang kita gunakan untuk intsall composer nya ( yang dibutuhkan yaitu php nya )

Sekarang Kita coba dulu apakah php di xampp bisa kita gunakan command nya... ,teman teman coba dulu mengetikan  perintah ( php -v ) untuk mengetest saja. bila mana mendapati tampilan seperti ini atau output seperti gambar di bawah maka php kamu sudah terinstall
!['Gambar Cek Version Php'](https://raw.githubusercontent.com/Ghonge1337/rysnanto/main/static/images/php-v.png)

jika muncul error, "php not blablabla" maka command php belum terdeteksi secara keseluruhan.Kita tambahkan sebuah environment baru didalam path. bagaimana caranya? teman teman klick windows pada keyboard lalu ketikan "edit Environtment Variabel" maka akan muncul app nya , tingaal klick 2 kali maka akan masuk ke app nya. setelah itu klick button "Environtmen Variabel", 
!['Edit Environment'](https://raw.githubusercontent.com/Ghonge1337/rysnanto/main/static/images/setupvariabel.png)
Setelah itu teman teman klick path pada system variabel setelah itu edit.
!['Edit Environment'](https://raw.githubusercontent.com/Ghonge1337/rysnanto/main/static/images/newenv.png)
tambahkan variabel baru (C:\xampp\php) tanpa tanda kurung setelah itu pilih oke, selesai... cek kembali dengan mengetikan (php -v)

Oke sekarang teman-teman tinggal download aplikasi composer , link download ada diaas atau melalui website resmi composer.Jika sudah terunduh klick 2 kali aplikasi setup nya. di tampilan pertama kita di suguhkan dengan opsi untuk developer atau tidak,kita klick next saja.
!['Gambar Install Composer'](https://raw.githubusercontent.com/Ghonge1337/rysnanto/main/static/images/composerinstall.png)
Setelah itu otomatis akan ke include php yang berada di folder (C:\xampp\php\php.exe) , jika belum otomatis terinclude teman teman bisa klick browse dan masuk ke folder diatas. atau ingin pakai php sendiri selain dari xampp juga boleh..., setelah itu klick next saja dan tunggu proses install selesai.
!['Gambar Install Composer'](https://raw.githubusercontent.com/Ghonge1337/rysnanto/main/static/images/composerinstall2.png)

Jika sudah maka kita tinggall mengetikan command di bawah untuk membuat sebuah project laravel
```php
composer create-project laravel/laravel namaproject
```
