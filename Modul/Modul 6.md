# Praktikum Modul 6 - Model, Controller dan Request-Response Handler

## Model
* ### Langkah 1
Membuat model User.php menggunakan php artisan make:model User. Setelah model dibuat, hapus kode sebelumnya dan ganti menjadi seperti berikut:
![img1](../screenshot/6-2.png)

## Controller
* ### Langkah 1
Membuat salinan ExampleController.php dan memberi nama salinan HomeController.php. Pada HomeController.php dibuat fungsi index() seperti berikut:
![img1](../screenshot/6-1b.png)
* ### Langkah 2
Mengubah route pada file web.php sehingga menjadi seperti berikut:
![img1](../screenshot/6-2b.png)
* ### Langkah 3
Menjalankan aplikasi dengan php -S localhost:8000 -t public. Saat aplikasi dijalankan, maka web browser akan mengeluarkan pesan berikut
![img1](../screenshot/6-3b.png)

## Request Handler
* ### Langkah 1
Melakukan import library Request dan melakukan perubahan fungsi index() pada HomeController.php
![img1](../screenshot/6-1c2.png)
* ### Langkah 2
Menjalankan aplikasi
![img1](../screenshot/6-2c.png)

## Response Handler
* ### Langkah 1
Melakukan import library Response di HomeController.php
![img1](../screenshot/6-1d.png)
* ### Langkah 2
Membuat fungsi Hello(), sehingga keseluruhan code menjadi seperti berikut:
![img1](../screenshot/6-2d.png)
* ### Langkah 3
Menambahkan route hello pada web.php
![img1](../screenshot/6-3d.png)
* ### Langkah 4
Menjalankan aplikasi pada route hello
![img1](../screenshot/6-4d.png)

## Penerapan
* ### Langkah 1
Melakukan import Model Users pada bagian atas HomeController.php
![img1](../screenshot/6-1e.png)
* ### Langkah 2
Menambahkan 3 fungsi baru di HomeController.php
![img1](../screenshot/6-2e.png)
* ### Langkah 3
Menambahkan 3 route baru di web.php
![img1](../screenshot/6-3e.png)
* ### Langkah 4
Menjalankan aplikasi melalui postman
route users/default (POST)
![img1](../screenshot/6-4e1.png)

route users/all (GET)
![img1](../screenshot/6-4e2.png)

