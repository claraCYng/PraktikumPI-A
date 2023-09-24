# Praktikum Modul 3 - Integrasi MongoDB dan Express

## Percobaan Instalasi NodeJs
* ### Langkah 1
> Mengunjungi halaman https://nodejs.org/en/
![img1](../screenshot/3-1.png)
* ### Langkah 2
> Download dan instal NodeJS, di sini saya menggunakan versi 20.7.0
![img1](../screenshot/3-2.png)
* ### Langkah 3
> Instalasi berhasil dan melakukan pengecekan versi
![img1](../screenshot/3-3.png)

## Inisiasi project Express dan pemasangan package
* ### Langkah 1
> Membuat folder express-mongodb
![img1](../screenshot/3-1b.png)
* ### Langkah 2
> Melakukan npm init untuk mengenerate file package.json
![img1](../screenshot/3-2b.png)
* ### Langkah 3
> Menginstal express, mongoose, dan dotenv
![img1](../screenshot/3-3b.png)

## Koneksi Express ke MongoDB
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
* ### Langkah 5
> Melakukan perubahan pada fungsi getAllBooks
![img1](../screenshot/3-5g.png)
* ### Langkah 6
> Melakukan perubahan pada fungsi getOneBooks
![img1](../screenshot/3-6g.png)
* ### Langkah 7
> lorem ipsum
![img1](../screenshot/3-.png)
* ### Langkah 8
> lorem ipsum
![img1](../screenshot/3-.png)
* ### Langkah 9
> Melakukan perubahan pada fungsi updateBook
![img1](../screenshot/3-9g.png)
* ### Langkah 10
> lorem ipsum
![img1](../screenshot/3-.png)
* ### Langkah 11
> Melakukan perubahan pada fungsi deleteBook
![img1](../screenshot/3-11g.png)
* ### Langkah 12
> lorem ipsum
![img1](../screenshot/3-.png)
