# Praktikum Modul 7 - Relasi One-to-Many dan Many-to-Many

## Pembuatan Tabel
* ### Langkah 1
Mengaktifkan server database (XAMPP) dan membuat database baru bernama lumenpost
![img1](../screenshot/7-1.png)
* ### Langkah 2
Mengubah konfigurasi database di .env sehingga database menjadi lumenpost
![img1](../screenshot/7-2.png)
* ### Langkah 3
Mengaktifkan beberapa library di file app.php
![img1](../screenshot/7-3.png)
* ### Langkah 4
Membuat file migration dengan command php artisan make:migration untuk membuat tabel posts, comments, tags, dan post comment 
![img1](../screenshot/7-4.png)
* ### Langkah 5
Mengubah fungsi up() di migrasi create_posts_table
![img1](../screenshot/7-5.png)
* ### Langkah 6
Mengubah fungsi up() di migrasi create_comments_table
![img1](../screenshot/7-6.png)
* ### Langkah 7
Mengubah fungsi up() di migrasi create_tags_table
![img1](../screenshot/7-7.png)
* ### Langkah 8
Mengubah fungsi up() di migrasi create_post_tag_table
![img1](../screenshot/7-8.png)
* ### Langkah 9
Menjalankan command php artisan migrate
![img1](../screenshot/7-9.png)

Ini tampilan di phpMyAdmin
![img1](../screenshot/7-92.png)


## Pembuatan Model
* ### Langkah 1
Membuat file di folder model dengan nama Post.php
![img1](../screenshot/7-1b.png)
* ### Langkah 2
Membuat file di folder model dengan nama Comment.php
![img1](../screenshot/7-2b.png)
* ### Langkah 3
Membuat file di folder model dengan nama Tag.php
![img1](../screenshot/7-3b.png)

## Relasi one to many
* ### Langkah 1
Menambahkan fungsi comment() di file Post.php
![img1](../screenshot/7-1c.png)
* ### Langkah 2
Menambhakan fungsi post() dan atribut postId pada fillable di file Post.php
![img1](../screenshot/7-2c.png)
* ### Langkah 3
Membuat file PostController.php di folder controller
![img1](../screenshot/7-3c.png)
* ### Langkah 4
Membuat file CommentController.php di folder controller
![img1](../screenshot/7-4c.png)
* ### Langkah 5
Menambahkan route baru di web.php
![img1](../screenshot/7-5c.png)
* ### Langkah 6
Mengisi value dari content dengan "disana engkau berdua" dan melakukan post di postman
![img1](../screenshot/7-6c.png)
* ### Langkah 7
Membuat komen dan melakukan post di route /comments
![img1](../screenshot/7-7c.png)
* ### Langkah 8
Menampilkan post dengan id 1 di postman
![img1](../screenshot/7-8c.png)

## Relasi many to many
* ### Langkah 1
Menambahkan fungsi tags() di Post.php
![img1](../screenshot/7-1d.png)
* ### Langkah 2
Menambahkan fungsi posts() di Tag.php
![img1](../screenshot/7-2d.png)
* ### Langkah 3
Membuat file TagController.php
![img1](../screenshot/7-3d.png)
* ### Langkah 4
Menambahkan fungsi addTag() dan response() di PostController.php
![img1](../screenshot/7-4d.png)
* ### Langkah 5
Menambahkan route baru di web.php
![img1](../screenshot/7-5d.png)
* ### Langkah 6
Membuat satu tag di Postman dengan route /tags
![img1](../screenshot/7-6d.png)
* ### Langkah 7
Menambahkan tag ke Post
![img1](../screenshot/7-7d.png)
* ### Langkah 8
Menampilkan Post
![img1](../screenshot/7-8d.png)
* ### Langkah 9
Membuat postingan di postman
![img1](../screenshot/7-9d.png)
* ### Langkah 10
Menambahkan tag dengan id 1 ke Post dengan id 2
![img1](../screenshot/7-10d.png)
* ### Langkah 11
Membuat tag "lagu" di postman
![img1](../screenshot/7-11d.png)
* ### Langkah 12
Menambahkan tag "lagu" ke post dengan id 2
![img1](../screenshot/7-12d.png)
* ### Langkah 13
Menampilkan Post pertama
![img1](../screenshot/7-13d.png)
* ### Langkah 14
Menampilkan Post kedua
![img1](../screenshot/7-14d.png)
