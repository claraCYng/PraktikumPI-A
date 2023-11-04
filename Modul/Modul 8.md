# Praktikum Modul 8 - Register, Authentication dan Authorization

## Register
* ### Langkah 1
Membuat file AuthController.php di folder Controller
![img1](../screenshot/8-3.png)
* ### Langkah 2
Menambahkan route baru di web.php 
![img1](../screenshot/8-4.png)
* ### Langkah 3
Menjalankan di postman dengan body seperti di gambar
![img1](../screenshot/8-5.png)


## Authentication
* ### Langkah 1
Menambahkan fungsi login di AuthController.php
![img1](../screenshot/8-1b.png)
* ### Langkah 2
Menambahkan route baru di web.php
![img1](../screenshot/8-2b.png)
* ### Langkah 3
Menjalankan di Postman dengan body seperti di gambar
![img1](../screenshot/8-3b.png)
Berikut jika password salah
![img1](../screenshot/8-3b2.png)

## Token
* ### Langkah 1
Membuat file migrasi baru
![img1](../screenshot/8-1c.png)
* ### Langkah 2
Menambahkan kode berikut di migrasi yang baru dibuat
![img1](../screenshot/8-2c.png)
* ### Langkah 3
Menambahkan atribut token di $fillable, sehingga kode menjadi seperti berikut
![img1](../screenshot/8-3c.png)
* ### Langkah 4
Menambahkan "$user->token = Str::random(36);" dan "$user->save()" di fungsi login pada AuthController seperti gambar berikut. Sebelumnya perlu mengimpor Str terlebih dahulu
![img1](../screenshot/8-4c.png)
impor Str
![img1](../screenshot/8-4c2.png)
* ### Langkah 5
Menjalankan php artisan migrate
![img1](../screenshot/8-5c.png)
* ### Langkah 6
Menjalankan di Postman, terlihat token sudah muncul
![img1](../screenshot/8-6c.png)


## Authorization
* ### Langkah 1
Membuat file Authorization.php di folder Middleware
![img1](../screenshot/8-1d.png)
* ### Langkah 2
Menambahkan middleware baru
![img1](../screenshot/8-2d.png)
* ### Langkah 3
Menambahkan fungsi home di file HomeController.php
![img1](../screenshot/8-3d.png)
* ### Langkah 4
Menambahkan route baru di web.php
![img1](../screenshot/8-4d.png)
* ### Langkah 5
Menjalankan aplikasi di Postman dengan memasukkan token yang sudah didapatkan sebelumnya
![img1](../screenshot/8-5d.png)

