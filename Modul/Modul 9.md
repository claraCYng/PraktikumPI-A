# Praktikum Modul 8 - JSON Web Token

## Penyesuaian Database
* ### Langkah 1
Menghapus parameter 72 di function up() pada file migrasi AddToken, sehingga function menjadi seperti ini:
![img1](../screenshot/9-1.png)
* ### Langkah 2
Memperbarui migrasi sebelumnya
![img1](../screenshot/9-2.png)
* ### Langkah 3
Menjalankan di postman dengan body seperti di gambar
![img1](../screenshot/9-3.png)


## JWT Manual
* ### Langkah 1
Menambahkan 3 fungsi baru pada AuthController.php
![img1](../screenshot/9-1brev.png)
* ### Langkah 2
Mengubah fungsi login
![img1](../screenshot/9-2b.png)
* ### Langkah 3
Menambahkan 4 fungsi baru di file Authorization.php
![img1](../screenshot/9-3b.png)
* ### Langkah 4
Mengubah fungsi handle di file Authorization.php
![img1](../screenshot/9-4b.png)
* ### Langkah 5
Menjalankan di Postman dengan body seperti berikut
![img1](../screenshot/9-5b.png)
Dan hasilnya seperti ini
![img1](../screenshot/9-5b2.png)
Terdapat informasi token, lalu token disalin ke notepad
* ### Langkah 6
Jalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat setelah login pada header
![img1](../screenshot/9-6b.png)

## JWT Library
* ### Langkah 1
Generate secret key di website Dejcrety
![img1](../screenshot/9-1c.png)
Memasukkan secret key yang didapatkan ke file .env
![img1](../screenshot/9-1c3.png)
* ### Langkah 2
Menginstal package jwt firebase
![img1](../screenshot/9-2c.png)
* ### Langkah 3
Menambahkan fungsi baru di AuthContrller.php
![img1](../screenshot/9-3c.png)
* ### Langkah 4
Mengubah fungsi login dan menghapus 3 fungsi sebelumnya
![img1](../screenshot/9-4crev.png)
* ### Langkah 5
Membuat file middleware bernama JwtMiddleware.php
![img1](../screenshot/9-5c.png)
* ### Langkah 6
Mendaftarkan middleware di app.php
![img1](../screenshot/9-6c.png)
* ### Langkah 7
Menambahkan doute baru di web.php
![img1](../screenshot/9-7c.png)
* ### Langkah 8
Menjalankan di Postman dengan body sebagai berikut
![img1](../screenshot/9-8c.png)
Terlihat hasil dan token sebagai berikut
![img1](../screenshot/9-8c2.png)
* ### Langkah 9
Menjalankan aplikasi di /home dengan memasukkan token yang sudah didapatkan sebelumnya
![img1](../screenshot/9-9c.png)


