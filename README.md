# FINAL PROJECT OS ADMIN - WEB SERVER

# A. Apa Itu Web Server?
Web server adalah perangkat lunak atau perangkat keras yang melayani permintaan dari klien (browser) untuk mengakses halaman web. Fungsi utama adalah menyajikan halaman web, dokumen, gambar, atau data lain kepada pengguna melalui protokol HTTP. Terdapat 3 peran web server, yaitu :

• Mengelola permintaan dari klien.

• Menyediakan akses ke berkas-berkas yang di-host.

• Menangani protokol HTTP dan HTTPS.

# B. Persiapan Pembuatan Web Server
Hal - hal utama yang perlu disiapkan dalam pembuatan Web Server :
•	Sistem Operasi : Instalasi dan konfigurasi sistem operasi server, seperti Ubuntu Server, CentOS, atau Windows Server.

•	Perangkat Lunak Web Server : Pilih web server seperti Apache, Nginx, dll. Kita instalasikan serta konfigurasikan sesuai kebutuhan.

•	Database Server : Jika diperlukan, instalasikan dan konfigurasikan database server seperti MySQL, MariaDB, dll.

•	Bahasa Pemrograman & Framework : Persiapkan bahasa pemrograman seperti PHP, Python, dll serta framework yang diperlukan untuk pengembangan aplikasi web.

•	Keamanan : Terapkan tindakan keamanan, termasuk pengaturan firewall, pembaruan perangkat lunak dan penggunaan SSL/TLS.


# C. Langkah - Langkah Membuat Web Server :

1. Instalasi Ubuntu Server
Download dan instalasikan Ubuntu Server di ubuntu.com/download/server

2. Update Sistem
Jalankan perintah sudo apt update untuk memastikan sistem diperbarui.

3. Instalasi Web Server (Apache)

•	Buka terminal dan jalankan perintah berikut :
sudo apt install apache2

•	Mulai dan aktifkan Apache :
sudo systemctl start apache2
sudo systemctl enable apache2

4. Instalasi Database Server MariaDB

•	Instal Database Server MariaDB
sudo apt install mariadb-server (untuk MariaDB)

•	Jalankan perintah keamanan untuk mengamankan database :

Untuk MariaDB: sudo mysql_secure_installation

5. Instalasi PHP

•	Install PHP dan modul yang diperlukan, lalu restart Apache untuk menerapkan perubahan:
sudo apt install php libapache2-mod-php php-mysql
sudo systemctl restart apache2

6. Instalasi SSH (Secure Shell) biasanya sudah diinstal di Ubuntu Server secara default. Untuk memeriksa apakah SSH sudah terinstal, bisa jalankan command ssh -V. Jika SSH sudah terinstal, akan ada versi SSH yang berjalan.

# D. Kesimpulan
Dalam Progress Final Project kali ini, saya telah melakukan instalasi fitur-fitur yang akan diperlukan untuk mengelola situs web secara dinamis di Ubuntu Server, seperti Apache, MariaDB, PHP, dan SSH. Meskipun ada beberapa masalah/error yang muncul selama proses instalasi. Saat ini, saya sedang menjalani tahap awal dalam pengembangan situs web dinamis ini dan akan terus mengembangkan-nya dan mengoptimalkan-nya, sehingga bisa mencapai tujuan proyek dengan baik. Aamiin. Kedepan saya akan membuat sebuah Web Server yang berisikan Musik dan Gambar dari vokalis favorit saya yaitu Ari Lasso (semoga bisa).
