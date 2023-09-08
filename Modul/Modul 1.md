# Praktikum Modul 1 - Instalasi Lumen, MongoDB dan Konfigurasi APP Key

## 1. Menginstal PHP
![img1](screenshot/php.png)
PHP berhasil diinstal di perangkat dengan versi PHP 8.0.30

## 2. Menginstal Composer
![img1](screenshot/composer.png)
Agar berhasil melakukan instalasi Composer, PHP harus sudah terinstal terlebih dahulu. Di gambar terlihat bahwa Composer sudah berhasil diinstal

## 3.Menginstal MongoDB
![img1](screenshot/mongo.png)
MongoDB berhasil terinstal ditandai dengan MongoDB Compass yang terbuka otomatis

## 4. Menginstal Lumen
### a. Lumen terinstal
![img1](screenshot/lumenapi.png)
![img1](screenshot/direktori.png)
Sebelumnya Lumen telah terinstal dan tersimpan pada direktori seperti gambar di atas
### b. Menjalankan server lumen
![img1](screenshot/server.png)
Setelah berhasil menginstal Lumen, kemudian menjalankan server lumen

## 5. Konfigurasi APP_KEY
Dalam hal ini saya tidak menggunakan Laravel tetapi menggunakan Lumen, sehingga untuk men-generate APP_KEY menggunakan langkah berikut:
### a. Membuka file web.php dan menambahkan random string sepanjang 32
![img1](screenshot/endpoint.png)
### b. Generate string di website https://pinetools.com/random-string-generator
![img1](screenshot/pinetools.png)
### c. Memasukkan random string ke file .env
![img1](screenshot/enc.png)



