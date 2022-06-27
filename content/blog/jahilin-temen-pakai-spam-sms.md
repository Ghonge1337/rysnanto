+++
date = 2022-06-26T17:00:00Z
description = "Jika kamu gabut atau memang jahil bisa nih di coba script python untuk spam sms"
draft = true
image = ""
title = "Jahilin temen pakai spam sms"

+++
**Disclaimer** : Gunakan dengan sewajar nya , jangan berlebih-lebihan.**"Hai Ahli Kitab, janganlah kamu berlebih-lebihan (melampaui batas) dengan cara tidak benar dalam agamamu. Dan janganlah kamu mengikuti hawa nafsu orang-orang yang telah sesat dahulu (sebelum kedatangan Muhammad) dan mereka telah menyesatkan kebanyakan (manusia), dan mereka tersesat dari jalan yang lurus.**” (**QS Al-Maidah:77**).

## Install Termux

Kenapa kok Termux? Ya karena audiens penonton saya rata rata menggunakan android hehehe, buat teman-teman yang pakai laptop caranya sama, tinggal download saja python di laptop teman teman. Dan install semua modules yang dibutuhkan di codingan spam sms ini.

## Clone Repository

Sebelum menjalankan program nya teman teman terlebih dahulu file program nya di github saya, untuk cara clone nya harus terlebih dahulu meng-install git cli di Termux. Untuk cara instalasi git sudah ada di blog saya ini, atau jika teman-teman malas mencari artikel nya bisa klick link berikut ini

[https://www.rysnanto.eu.org/blog/install-github-cli-di-termux/](https://www.rysnanto.eu.org/blog/install-github-cli-di-termux/ "https://www.rysnanto.eu.org/blog/install-github-cli-di-termux/")

Saya anggap teman-teman sudah meng-installnya mari kita clone repo saya dengan cara ketikan perintah di bawah ini

    git clone https://github.com/Ghonge1337/spam.git

Jika sudah maka secara otomatis di Termux teman-teman terdapat folder spam , cek aja menggunakan perinta **ls.**

## **Install Python**

Setelah selesai clone repo saya , kita akan install Python dulu agar bisa menjalankan program spam sms nya. Untuk menginstall python teman-teman bisa mengetikkan perintah di bawah ini

    pkg install python

Dengan perintah tersebut maka akan mengunduh python dengan ukuran 456mb kalo gak salah. Tunggu saja hingga proses selesai.

## Install Module

Program spam ini perlu module tambahan agar dapat di jalankan , apabila belum atau tidak maka program tidak berjalan dan mengalami error. Di program spam ini hanya memerlukan 2 module saja mari kita install. Pastekan saja perintah di bawah ini.

    pip install requests

    pip install colorama