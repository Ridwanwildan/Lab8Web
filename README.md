# :rocket: Latihan CRUD Sederhana

Made With : [![Google Chrome](https://img.shields.io/badge/Google_chrome-4285F4?style=for-the-badge&logo=Google-chrome&logoColor=white)](https://www.google.com/intl/id_id/chrome/) [![Visual Studio Code](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com/) [![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)

- Nama : Hizbullah Ridwan
- NIM : 312110055
- Kelas : TI.21.B.1
- Mata Kuliah : Pemrograman Web

Daftar isi :

- [Run MYSQL Server](https://github.com/Ridwanwildan/Lab8Web#run-mysql-server)
- [Run Web Server](https://github.com/Ridwanwildan/Lab7Web#run-web-server)
- [Create Folder and File](https://github.com/Ridwanwildan/Lab7Web#create-folder-and-file)
- [Hello World](https://github.com/Ridwanwildan/Lab7Web#hello-world)
- [Variable](https://github.com/Ridwanwildan/Lab7Web#variable)
- [Predefine Variable GET](https://github.com/Ridwanwildan/Lab7Web#predefine-variable-get)
- [Create Form Input](https://github.com/Ridwanwildan/Lab7Web#create-form-input)
- [Operator](https://github.com/Ridwanwildan/Lab7Web#operator)
- [Conditional](https://github.com/Ridwanwildan/Lab7Web#conditional)
- [Loop](https://github.com/Ridwanwildan/Lab7Web#loop)
- [Tugas](https://github.com/Ridwanwildan/Lab7Web#tugas)

## Run MYSQL Server

Pertama adalah melakukan running pada MYSQL server. Caranya adalah buka [XAMPP](https://www.apachefriends.org/) control kemudian pilih start pada `apache` dan `MySQL`. Kemudian untuk memastikan bahwa MYSQL server sudah running, akses ke `http://localhost` atau `http://127.0.0.1` pada browser.

![Gambar 1](Screenshoots/Capture1.PNG)

## Go To PHPMyAdmin

Setelah pertama sudah berhasil running MYSQL server, selanjutnya adalah mengakses PHPMyAdmin di `http://localhost/phpmyadmin`. Akan terlihat menu utama dari PHPMyAdmin dan beberapa database yang sudah ada pada komputer.

### Create Database

Kemudian buat database baru menggunakan query dengan nama `latihan1`. Seperti ini :

```bash
CREATE DATABASE latihan1;
```

![Gambar 2](Screenshoots/Capture2.PNG)

### Create Table

Pada latihan kali ini, Studi kasusnya adalah Data Barang. Maka buatlah tabel dengan nama `data_barang` dan dengan query seperti ini :

```bash
CREATE TABLE data_barang (
 id_barang int(10) auto_increment Primary Key,
 kategori varchar(30),
 nama varchar(30),
 gambar varchar(100),
 harga_beli decimal(10,0),
 harga_jual decimal(10,0),
 stok int(4)
);
```

![Gambar 3](Screenshoots/Capture3.PNG)

Klik Go dan hasilnya bisa dilihat pada table structure.

![Gambar 4](Screenshoots/Capture4.PNG)

### Add Data

Setelah tabel berhasil dibuat maka tabel tersebut masih kosong. Isi tabelnya dengan query seperti ini :

```bash
INSERT INTO data_barang (kategori, nama, gambar, harga_beli, harga_jual, stok)
VALUES ('Elektronik', 'HP Samsung Android', 'hp_samsung.jpg', 2000000, 2400000, 5),
('Elektronik', 'HP Xiaomi Android', 'hp_xiaomi.jpg', 1000000, 1400000, 5),
('Elektronik', 'HP OPPO Android', 'hp_oppo.jpg', 1800000, 2300000, 5);
```

Hasilnya bisa dilihat di menu `browse`.

![Gambar 5](Screenshoots/Capture5.PNG)
