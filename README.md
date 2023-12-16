# FINAL PROJECT OS ADMIN - WEB SERVER

# A. Apa Itu Web Server?
Web server adalah perangkat lunak atau perangkat keras yang melayani permintaan dari klien (browser) untuk mengakses halaman web. Fungsi utama adalah menyajikan halaman web, dokumen, gambar, atau data lain kepada pengguna melalui protokol HTTP. Terdapat 3 peran web server, yaitu :

1. Mengelola permintaan dari klien.
1. Menyediakan akses ke berkas-berkas yang di-host.
1. Menangani protokol HTTP dan HTTPS.

# B. Persiapan Pembuatan Web Server
Hal - hal utama yang perlu disiapkan dalam pembuatan Web Server :

  -	**Sistem Operasi** :
    > Instalasi dan konfigurasi sistem operasi server, pada kali ini menggunakan `Ubuntu Server`

  -	**Perangkat Lunak Web Server** :
    > Pilih web server yang pada kali ini kita gunakan `Apache`

  -	**Database Server** :
    > Jika diperlukan, instalasikan dan konfigurasikan database server yang pada kali ini kita gunakan `MariaDB`

  -	**Bahasa Pemrograman** :
    > Persiapkan bahasa pemrograman yang pada kali ini kita gunakan `PHP`

  -	**Keamanan** :
    > Terapkan tindakan keamanan, termasuk pengaturan firewall, pembaruan perangkat lunak dan penggunaan `SSL/TLS`


# C. Tools Yang Wajib di Install dalam Web Server :

## - Instalasi Ubuntu
Download dan instal Ubuntu di `ubuntu.com/download`

## - Update Sistem
Jalankan perintah `sudo apt update` untuk memastikan sistem diperbarui.

## - Instalasi Web Server (Apache)

Buka terminal dan jalankan perintah berikut :
  - `sudo apt install apache2`

Mulai dan aktifkan Apache :
  - `sudo systemctl start apache2`
  - `sudo systemctl enable apache2`

## - Instalasi Database Server MariaDB

Instal Database Server MariaDB
  - `sudo apt install mariadb-server` (untuk MariaDB)

Jalankan perintah keamanan untuk mengamankan database :

  - Untuk MariaDB : `sudo mysql_secure_installation`

## - Instalasi PHP

Install PHP dan modul yang diperlukan, lalu restart Apache untuk menerapkan perubahan:
  - `sudo apt install php libapache2-mod-php php-mysql`
  - `sudo systemctl restart apache2`

## - Instalasi SSH (Secure Shell)

Biasanya sudah diinstal di Ubuntu Server secara default. Untuk memeriksa apakah SSH sudah terinstal, bisa jalankan command `ssh -V`

## - Instalasi WinSCP untuk Memasukkan HTML & CSS

Download dan instal di `winscp.net/eng/downloads.php`

# D. Cara Memasukkan HTML & CSS Menggunakan WinSCP

Berikut step by step memasukkan HTML & CSS di WinSCP :
1. s
1. s
1. s
1. s
1. s
1. s
1. s
1. s


# E. Kesimpulan
Dalam Progress Final Project kali ini, saya telah melakukan sejumlah langkah yang membuahkan hasil sesuai harapan. Tema web server biografi tokoh yang berfokus pada musik dengan menampilkan embeb link Spotify dan gambar dari vokalis favorit saya, `Ari Lasso` berhasil diimplementasikan dengan baik. Selama proses ini, saya berhasil mengatasi kendala yang muncul, terutama terkait dengan penggantian alamat IP agar dapat diakses melalui browser setelah menginstall Apache. Keberhasilan ini memastikan bahwa web server dapat diakses dengan lancar. Hasil akhir proyek mencakup penyelarasan HTML & CSS untuk merinci biografi tokoh dan menghadirkan tampilan yang estetis dan informatif. Kedepannya, proyek ini akan terus dikembangkan untuk meningkatkan fungsionalitas dan estetika.
