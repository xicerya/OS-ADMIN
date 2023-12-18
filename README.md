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
1. Pastikan sudah menginstall **Apache** dan Update Sistem Terbaru seperti yang sudah ada diatas.
1. Kemudian ketik command : `ls /var/www/html/`
   > Pastikan disitu akan ada `index.html`
1. Lalu, jalan command : `cat /var/www/html/index.html`
   > Command diatas Untuk melihat apa isi file yang ada.
1. Carilah Template CSS di `www.free-css.com` dan Download + Ekstrak folder file dimanapun (bebas) untuk dimasukkan ke Web Server.
   > Disini kita bisa cari web seperti apa yang kita inginkan dan bisa kita edit sendiri melalui **Visual Studio Code**.
   > Kebetulan kali ini sudah saya edit isinya sekaligus nama filenya dengan **arilasso**.
1. Buka **WinSCP** yang kita Install tadi. Plih **New Site**.
1. Kita diperintahkan untuk memasukkan Hostname, Username dan Password Server yang kita buat sebelumnya. Lalu, klik **Login** dan **Yes**.
1. Setelah memasukkan Hostname, Username dan Password Server kita bisa melihat folder Home dari Server tersebut.
1. Kemudian Cari dan Drag folder file HTML & CSS yang sudah kita edit di VS Code ke Home dari Server tersebut.
1. Untuk mengecek apakah file sudah dimasukkan atau belum, kita harus kembali lagi ke Server lalu masukkan command : `ls`
   > Pastikan ada nama folder file yang sudah di Drag tadi.
1. Sekarang kita hapus default page Apache-nya dengan command :
   - `cd /var/www/html/`
   - `ls` : Untuk mengecek untuk file yang ada yaitu index.html
   - `sudo rm index.html`
     > Dan disini folder dipastikan kosong.
1. Setelah itu kita copy folder file HTML & CSS yang sudah kita drag ke Home Server dengan command : `sudo cp -r ~/arilasso/* .`
1. Kemudian kita masukkan command `ls` lagi
1. Terakhir, masukkan IP Address dari Server kita, yang kebetulan IP Address kita kali ini adalah : `192.168.1.20`
1. Dan akan muncul halaman website dari folder file HTML & CSS yang sudah kita edit di VS Code.
   <img width="69" alt="Untitled" src="https://github.com/xicerya/OS-ADMIN/assets/145538720/96522ecb-e547-48c0-bd92-d24fc446f244">
1. **SELESAI**


# E. Kesimpulan
Dalam Progress Final Project kali ini, saya telah melakukan sejumlah langkah yang membuahkan hasil sesuai harapan. Tema web server yang saya ambil adalah biografi tokoh yang berfokus pada musik dengan menampilkan embeb link Spotify dan gambar dari vokalis favorit saya, yaitu **Ari Lasso**. Telah berhasil diimplementasikan dengan baik. Selama proses ini, saya berhasil mengatasi kendala yang muncul, terutama terkait dengan penggantian alamat IP agar dapat diakses melalui browser setelah menginstall Apache dengan command `sudo nano 01-netcfg.yaml`. Keberhasilan ini memastikan bahwa web server dapat diakses dengan lancar. Hasil akhir proyek mencakup penyelarasan HTML & CSS untuk merinci biografi tokoh dan menghadirkan tampilan yang informatif. Kedepannya, proyek ini akan terus dikembangkan untuk meningkatkan fungsionalitas.

# F. Refrensi Pembuatan Web Server
Terdapat refrensi yang saya dapat dalam pembuatan Web Server, yaitu :
1. Channel YouTube : **Abstract programmer**
   > Link Video : https://youtu.be/PZAT0tIwYh4?si=wrRMgQI20tAwcUQL
1. ChatGPT
