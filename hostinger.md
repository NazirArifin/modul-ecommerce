# Hosting [idhostinger](https://www.hostinger.co.id/) & Instalasi Wordpress

![idhostinger](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger_zpsicke52se.png "hostinger.co.id")

## Tahap Persiapan

* Pastikan Anda sudah terdaftar dan mempunyai akun di hosting idhostinger. Kemudian akses halaman [__LOGIN__](https://cpanel.idhostinger.com/auth) dan masukkan email serta password yang Anda miliki.

![login](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-login_zpslqc0vbnw.png "halaman login")

## Pembuatan Free Hosting

* Setelah masuk, Anda akses menu __HOSTING__ di bagian atas halaman untuk melakukan manajemen hosting.
* Buat hosting baru dengan menekan tombol __New Hosting Account__ / __Order Hosting Baru__. Untuk ujicoba pada tampilan berikutnya Anda pilih _Free Plan_ atau _Gratis_. 
* Lanjutkan proses dengan menekan tombol __Checkout__ di sisi kanan dan dilanjutkan dengan menekan tombol __Submit Order__.

![checkout](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-checkout_zpsto6z1ewl.png "order checkout")

## Manajemen Hosting
* Selanjutnya di proses __Pengaturan Order Hosting__ untuk mendapatkan alamat subdomain hosting gratis Anda, pilih _Subdomain Gratis_ untuk pilihan Jenis Domain, kemudian masukkan nama subdomain yang Anda inginkan, centang lokasi server Eropa dan isi password sesuai dengan password yang Anda miliki.

![hosting](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-hosting_zpsoweur11z.png "create hosting")

* Coba akses alamat subdomain Anda sesuai dengan nama yang Anda masukkan dan Anda akan melihat tampilan "__Akun Anda telah dibuat__".

![created](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-created_zps0leq9ii4.png "created")

* Kembali ke menu __HOSTING__ dan klik subdomain yang sudah Anda buat dan lanjutkan dengan menekan tombol __Kelola__.

![manage](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-manajemen_zpslufqkolv.png "manage")

## File Transfer Protocol
* Untuk manajemen file kita akan menggunakan FTP karena lebih mudah dan sederhana.
* _Scroll_ kebawah sampai menemukan menu __Akses FTP__. Kita akan mencoba mengupload satu berkas menggunakan FTP dan aplikasi [FileZilla](https://filezilla-project.org/).
* Buka aplikasi FileZilla dan di menu _File_ pilih _Site Manager_ dan _New Site_. Isikan konfigurasi FTP di hosting Anda ke FileZilla. Setelah lengkap tekan tombol _Ok_.

![ftp](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-ftp_zpsllnl9fpd.png "setting ftp")

* Coba lakukan koneksi ke server dengan menekan tombol _Site Manager_ yang ada dibawah menu file. Jika berhasil maka akan muncul daftar file yang ada server.

![ftp](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-ftp-work_zpsio2o3had.png "view ftp")

* Untuk ujicoba, buat sebuah file __index.php__ dengan isi:
```php
<?php
echo 'hello world';

```
* Upload file tersebut cara melakukan _drag & drop_ file dari folder lokal ke server. Setelah berhasil coba _refresh_/_reload_ halaman web Anda.

## Instalasi Wordpress
* Kita akan menggunakan Wordpress untuk aplikasi e-commerce yang akan dibuat. Sebagian besar hosting telah menyediakan _auto installer_ yang tinggal diklik maka aplikasi otomatis terinstall lengkap dengan database yang digunakan. Idhostinger juga mendukung _auto installer_ ini dan Anda dapat mengaksesnya melalui menu _Auto Installer_.

![auto installer](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-menu-autoinstaller_zpsx0mbpfxu.png "auto installer")

![auto installer](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-autoinstaller_zpshqs3qhxo.png "auto installer")

* Di halaman berikutnya Anda cari aplikasi Wordpress lalu Anda klik. Isikan inputan yang diminta sesuai dengan yang Anda inginkan. 

![setting wp](http://i1380.photobucket.com/albums/ah186/nazir579/install-wp_zpsxistohhc.png "setting wp")

* Setelah berhasil Anda dapat mengakses halaman Administrator dengan alamat: __http://free.hosting.anda/wp-admin/__ (_*pastikan bagian __free.hosting.anda__ diganti dengan alamat hosting Anda yang sebenarnya_).

![wp-login](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-wpadmin_zpskxkjm9ub.png "login wpadmin")

* Login ke wp-admin dengan akun yang Anda buat sebelumnya dan jika berhasil Anda akan melihat menu Administrator dari aplikasi Wordpress Anda. Coba Anda hapus Post Hello World yang ada di Wordpress.

![wpadmin](http://i1380.photobucket.com/albums/ah186/nazir579/hostinger-wpadmin_zpsqxyjl3we.png "wpadmin")

## Instalasi plugin [WP e-Commerce](http://docs.wpecommerce.org/)
* Di menu _sidebar_ sebelah kiri klik bagian _Plugins_ dan kemudian klik menu _Add New_. Di bagian _Search plugins_ Anda masukkan kata e-Commerce hingga Anda menemukan plugin __WP e-Commerce__ dan tekan tombol _Install Now_.
* Setelah selesai Anda dapat mengakses toko online Anda dengan menggunakan menu __Setting__ > __Store__. Akan ada banyak sekali pengaturan yang dapat Anda ubah sesuai dengan kebutuhan toko online Anda seperti _currency_, dsb.
* Untuk menambahkan produk yang ingin Anda tawarkan Anda dapat menggunakan menu __Products__ di menu _sidebar_. Coba Anda tambahkan satu produk di toko online Anda dan kemudian _Refresh_/_Reload_ halaman web Anda.

## Tambahan Untuk Belajar
* Pelajari dan install plugin e-commerce lain selain WP e-commerce  [http://www.wpbeginner.com/plugins/best-wordpress-ecommerce-plugins-compared/](http://www.wpbeginner.com/plugins/best-wordpress-ecommerce-plugins-compared/)
* Ubah tampilan wordpress dan menggunakan menu __Theme__ 

# Terima Kasih


 

