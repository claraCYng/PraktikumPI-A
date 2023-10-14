# Praktikum Modul 4 - Basic Routing & Migration

## Get
* ### Langkah 1
> Menambahkan kode berikut pada akhir baris di file web.php yang terletak di folder routes. Setelah disimpan, jalankan server PHP dengan perintah "php -S localhost:8000 -t public"
![img1](../screenshot/4-1a.png)
* ### Langkah 2
> Setelah server berjalan, buka URL http://localhost:8000/get. Maka browser akan menampilkan pesan "GET" seperti yang telah ditambahkan pada file web.php sebelumnya.
![img1](../screenshot/4-1a2.png)

## POST, PUT, PATCH, DELETE, dan OPTIONS
* ### Langkah 1
> Menambahkan methode POST, PUT, PATCH, DELETE, dan OPTIONS di file web.php
![img1](../screenshot/4-1b.png)
* ### Langkah 2
> Menginstal ekstensi Thunder Client di VSCode. Setelah diinstal, melakukan request ke URL berdasarkan methodenya
![img1](../screenshot/4-1bput.png)
![img1](../screenshot/4-1bpost.png)
![img1](../screenshot/4-1bpatch.png)
![img1](../screenshot/4-1bdel.png)
![img1](../screenshot/4-1bopt.png)

## Migrasi Database
* ### Langkah 1
> Membuat database lumenapi
![img1](../screenshot/4-1c.png)
> Mengubah konfigurasi database pada file .env
![img1](../screenshot/4-1c2.png)
* ### Langkah 2
> Menghapus komen baris berikut di file app.php sehingga kode aktif, seperti di gambar
![img1](../screenshot/4-1c3.png)
* ### Langkah 3
> Menjalankan perintah berikut di terminal
![img1](../screenshot/4-1c4.png)
> Sehingga dihasilkan file berikut
![img1](../screenshot/4-1c4b.png)
* ### Langkah 4
> Mengubah code pada fungsi up() di create_table_user
![img1](../screenshot/4-1c5.png)
* ### Langkah 5
> > Mengubah code pada fungsi up() di create_product_table
![img1](../screenshot/4-1c6.png)
* ### Langkah 6
> > Mengubah perintah php artisan migrate di terminal
![img1](../screenshot/4rev1.png)
> > Berikut tampilannya di phpMyAdmin
![img1](../screenshot/4rev2.png)

