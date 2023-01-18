+++
date = 2023-01-16T17:00:00Z
description = "Tugas dari pak Slamet.SP.d"
image = ""
title = "membuat auth login multi user"

+++
[Rysnanto](rysnanto.eu.org) - Berikut ini merupakan rincian tugas membuat auth login dengan PHP native.

Logic

>     $data = mysqli_fetch_assoc($query);
>     if($data['role'] == "admin"){
>        $_SESSION = "admin";
>        ("Location: dashboard/index.php");
>     }else{
>        $_SESSION = "user";
>        header("Location: dashboard/index.php");
>     }

    