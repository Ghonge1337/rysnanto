+++
date = 2022-06-19T17:00:00Z
description = "Meng-install Github CLI di android lewat Termux"
image = "/uploads/images.jpeg"
title = "Install Github CLI di Termux"

+++
Disclaimer : _Gambar Thumbnail saya ambil dari website github. Github CLI akan kita install di Termux._

### **Pengertian Dan Definisi**

Github CLI itu - CLI sendiri merupakan pengertian Command Line Interface yang bisa kita simpulkan bahwa github CLI merupakan fitur yang biasa kita gunakan di website github namun kita juga bisa gunakan fitur tersebut melalui Command Line.

Termux sendiri merupakan terminal emulator layak nya cmd saat kita menggunakan windows. Saya yakin teman teman juga sudah menggunakan aplikasi ini itu berbagai hal. Nah pada artikel ini kita akan install Github CLI di Termux ini agar kita dapat melakukan interaksi dengan github di terminal android kita yaitu Termux.

### Instalasi

Teman - Teman download terlebih dahulu aplikasi Termux ini di playstore atau pun di google, terserah.Pokoknya harus install aplikasi ini dulu agar dapat mengikuti apa yang saya tulis.

Setelah berhasil meng-install aplikasi Termux silahkan di buka dan ketikkan perintah di bawah ini untuk menginstall github CLI nya.

```
pkg install git
```

Aku harap dlsetelah menuliskan perintah tersebut maka github CLI sudah terinstall, cara cek nya tinggal kita ketikan

```
git --version
```

### Masalah Error

Namun apabila teman teman menemui kendala seperti saya ini , berikut gambar error nya :

![](/uploads/screenshot_20220620-155048_peluncur_pixel.jpg)

Jangan panik terlebih dahulu , setelah saya cari cari penyebab nya akhir nya saya menemukan jawaban nya di stackoverflow [https://stackoverflow.com/questions/67647518/termux-repository-is-under-maintenance-or-down?rq=1](https://stackoverflow.com/questions/67647518/termux-repository-is-under-maintenance-or-down?rq=1 "https://stackoverflow.com/questions/67647518/termux-repository-is-under-maintenance-or-down?rq=1")

Teman-Teman bisa ketikkan perintah perintah di bawah ini untuk mengatasi error tersebut.

```
pkg remove game-repo
pkg remove science-repo
```

Jika ada peringatan (Y/N) ketik aja Y saja hingga akhir proses, jika sudah bagian akhir kita ketikkan lagi

```
pkg update
```

Maka akan ada proses update atau apa saya kurang paham yang sedang berjalan , jika ada peringatan lagi (Y/N) ketik saja Y hingga akhir proses berakhir. Dan ya semoga berhasil, sekarang tinggal kita ulangi lagi perintah untuk menginstall github CLI nya.

``` 
pkg install git
```

Nah itu dia bagaimana cara install Github CLI di Termux android , semoga berhasil bila mana ada kesulitan atau kendala sebaiknya tanya di komentar ataupun bisa mencari masalahnya di stackoverflow. Sekian terimakasih _^

### **Vidio Selama Saya Menemukan Error**

{{< youtube HpJqoPsZE94 >}}
