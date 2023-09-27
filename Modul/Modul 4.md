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
> Membuat file index.js
![img1](../screenshot/3-1c.png)
> Lalu menjalankan server node
![img1](../screenshot/3-1c2.png)
* ### Langkah 2
> Membuka file .env dan menambahkan kode seperti di gambar
![img1](../screenshot/3-2c.png)
* ### Langkah 3
> Menambahkan kode seperti di bawah pada file index.js
![img1](../screenshot/3-4c.png)
> Kemudian menjalankan aplikasi kembali
![img1](../screenshot/3-4c2.png)

## Pembuatan Routing
* ### Langkah 1
> Membuat folder routes dan membuat file bernama book.route.js. Pada file tersebut membuat kode seperti yang ada di gambar
![img1](../screenshot/3-4d.png)
* ### Langkah 2
> Melakukan import book.route.js di file index.js
![img1](../screenshot/3-5d.png)

## Pembuatan controller
* ### Langkah 1
> Membuat folder controllers dan membuat file book.controller.js. Kemudian membuat kode seperti di bawah
![img1](../screenshot/3-6e.png)
* ### Langkah 2
> Melakukan pengujian di Postman
![img1](../screenshot/3-7e.png)


## Pembuatan Model
* ### Langkah 1
> Membuat folder models dan membuat file book.model.js. Kemudian menambahkan baris kode berikut:
![img1](../screenshot/3.-3f.png)


## Operasi CRUD
* ### Langkah 1
> Menghapus data pada books colection
![img1](../screenshot/3-1g.png)
* ### Langkah 2
> Import book.model.js pada file book.controller.js, sehingga terdapat penambahan kode seperti di bawah:
![img1](../screenshot/3-2g.png)
* ### Langkah 3
> Mengubah fungsi create book
![img1](../screenshot/3-3g.png)
* ### Langkah 4
> Menambah daftar buku di Postman dengan data seperti di bawah:
![img1](../screenshot/3-4g.png)
![img1](../screenshot/3-4g2.png)
* ### Langkah 5
> Melakukan perubahan pada fungsi getAllBooks
![img1](../screenshot/3-5g.png)
* ### Langkah 6
> Melakukan perubahan pada fungsi getOneBooks
![img1](../screenshot/3-6g.png)
* ### Langkah 7
> Menampilkan semua buku yang telah ditambahkan sebelumnya
![img1](../screenshot/3-7g.png)
* ### Langkah 8
> Menampilkan buku Dilan 1990 dengan id "6513917e4ad6f77a40e4df70"
![img1](../screenshot/3-8g.png)
* ### Langkah 9
> Melakukan perubahan pada fungsi updateBook
![img1](../screenshot/3-9g.png)
* ### Langkah 10
> Mengubah judul buku DIlan 1991 dengan ID "651392164ad6f77a40e4df72" menjadi nama panggilan
![img1](../screenshot/3-10g.png)
* ### Langkah 11
> Melakukan perubahan pada fungsi deleteBook
![img1](../screenshot/3-11g.png)
* ### Langkah 12
> Menghapus buku Dilan 1990 dengan DELETE di Postman
![img1](../screenshot/3-12g.png)
