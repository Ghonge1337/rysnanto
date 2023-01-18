+++
date = 2023-01-16T17:00:00Z
description = "Tugas dari pak Slamet.SP.d"
image = ""
title = "membuat auth login multi user"

+++
[Rysnanto](rysnanto.eu.org) - Berikut ini merupakan rincian tugas membuat auth login dengan PHP native di Aplikasi Catatan Perjalanan kurang lebih seperti  Notepad. Sebelumnya di form login hanya bisa untuk 1 role saja yaitu penulis , sekarang tugas dari pak slamet membuat form login yang mampu Multi User ada admin dan User biasa.

**Demo** : [https://travel.jongnesia.com](https://travel.jongnesia.com)

untuk coba login :

**Username** : Rysnanto

**Password** : admin@rysnanto

## **Penjelasan**

Di bawah ini merupakan logika sederhana membuat multi user , logika nya masih ngawur dan untuk keamanan kurang begitu mengerti. Use your brains!

>     <?php
>     session_start();
>     include "../config.php";
>     if(isset($_POST['login'])){
>         $nik = mysqli_real_escape_string($konek , $_POST['nik']);
>         $username = mysqli_real_escape_string($konek , $_POST['username']);
>     
>     
>         $query = "SELECT * FROM pengguna WHERE nik='$nik' AND username='$username' ";
>         $login = mysqli_query($konek , $query);
>         $cek = mysqli_num_rows($login);
>         if($cek > 0){
>             $data = mysqli_fetch_assoc($login);
>             if($data['role'] == "admin"){
>                 $_SESSION['login'] = true;
>                 $_SESSION['username'] = $username;
>                 $_SESSION['nik_user'] = $nik;
>                 $_SESSION['role'] = $data['role'];
>                 $_SESSION['message'] = "Berhasil Login"; 
>                 header("location: ../dashboard/index.php");
>             }else{
>                 $_SESSION['login'] = true;
>                 $_SESSION['username'] = $username;
>                 $_SESSION['nik_user'] = $nik;
>                 $_SESSION['role'] = $data['role'];
>                 $_SESSION['message'] = "Berhasil Login"; 
>                 header("location: ../dashboard/index.php");
>             }
>         }else{
>             $_SESSION['message'] = "Gagal Login"; 
>             header("Location: ../login.php");
>         }
>     }