# Instalasi [OpenCart](https://www.opencart.com/)

![heroku](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-1_zpszh8qrwp2.png "opencart.com")

## Apakah OpenCart

> OpenCart is an online store management system. It is PHP-based, using a MySQL database and HTML components. Support is provided for numerous languages and currencies, and it is freely available under the GNU General Public License

---

## Tahap Persiapan
* Download atau clone OpenCart dari halaman [github](https://github.com/opencart/opencart). Didalamnya akan terdapat beberapa file dan  folder. File __"install.txt"__ berisi keterangan tentang bagaimana cara melakukan instalasi OpenCart sedangkan folder __"upload"__ adalah folder yang yang kita butuhkan dan akan diupload ke server.

* Kita akan melakukan instalasi secara _local_ di komputer kita dan tidak diupload ke server sehingga kita perlu mempersiapkan beberapa hal berhubungan dengan database yang akan digunakan.

* Buka [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/) dan buat sebuah database dengan nama __"tokoonline"__ atau nama lain sesuai keinginan Anda.

## Instalasi OpenCart (Local/Offline)

* Pindahkan folder __"upload"__ ke __htdocs__ atau jika Anda menggunakan _local server_ di PHP 5.6.x maka Anda dapat menjalankan server dengan perintah ```php -S localhost:8080```.

* Rename file __config-dist.php__ menjadi __config.php__ dan file __admin/config-dist.php__ menjadi __admin/config.php__.

* Akses dengan browser server localhost Anda dan Anda akan melihat tampilan instalasi yang terdiri dari 4 langkah. Langkah pertama adalah _License Agreement_, Anda dapat membacanya atau langsung saja menekan tombol __CONTINUE__.

![oc-step1](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-2_zps4akn7rhm.png "oc step1")

* Langkah berikutnya adalah pengecekan sistem oleh OpenCart, pastikan semua bagian memiliki status _checked_ dan file/folder memiliki status _Writeable_. Jika sudah tekan tombol __CONTINUE__.

![oc-step2](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-3_zpsu68ztbnv.png "oc step2")

![oc-step2.1](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-4_zps8b4ncz5i.png "oc step2.1")

* Langkah ketiga adalah pengisian _setting_ database. DB Driver pilih saja __MySQLi__. Database diisi dengan nama database yang telah Anda buat dari langkah sebelumnya. Bagian prefix bisa Anda kosongkan.

![oc-step3](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-5_zpsd4bv2asc.png "oc step 3")

* Selanjutnya masih di langkah ketiga terdapat bagian untuk login masuk aplikasi toko online Anda. Isi inputan tersebut sesuai dengan keinginan Anda. Tekan tombol __CONTINUE__ dan tunggu beberapa saat.

![oc-step3.1](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-6_zpskbfhko8j.png "oc step 3.1")

* Jika berhasil maka akan muncul pesan instalasi berhasil. Terdapat 2 link yang dapat Anda kunjungi yaitu halaman untuk mengakses toko online yang sudah Anda buat dan halaman administrator untuk mengakses halaman administrator toko online. Selamat Anda telah memiliki toko online yang sementara masih offline. Jangan lupa hapus folder __install__ setelah proses instalasi selesai.

![oc-finish](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-7_zpsatwjbaej.png "oc finish")

![oc-toko](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-8_zpszcegtxmk.png "oc dashboard")

![oc-toko](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-9_zps7r38foho.png "oc dashboard")

## Instalasi OpenCart (Online)

* Gunakan auto installer

## Ubah Profil Toko

* Pada menu sebelah kiri pilih __Settings__ dan Anda akan dibawa ke halaman pengaturan toko. Tekan tombol Edit di kolom Action. Anda dapat mengubah data Umum, Toko dll. Coba Anda ubah Nama toko, alamat toko dan pemilik toko lalu tekan tombol __Save__.

## Manajemen Extensions

* Extension adalah fitur tambahan yang dapat diinstall oleh pemilik toko untuk menambah fungsi-fungsi di tokonya. Anda dapat menggunakan menu Extensions di menu sebelah kiri untuk mengatur extension yang Anda gunakan.

![oc-setting](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-10_zpsdcjnapsr.png "oc setting")

### Mengubah Theme

* Cari theme _free_ di [OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_category_id=1&filter_license=free). Baca komentar untuk mengetahui apakah theme yang ditawarkan terdapat error atau tidak. Download theme yang Anda inginkan dan kemudian ekstrak folder __catalog__ dan __system__ ke direktori _root_. 

* Kemudian di pilih menu __Extensions__, pilih jenis extensionsnya __Theme__, kemudian bagian Your Store tekan tombol Edit. Setelah itu pilih theme yang Anda gunakan lalu tekan Save. Jika berhasil maka tampilan toko Anda sudah berubah.

![oc-theme](http://i1380.photobucket.com/albums/ah186/nazir579/oc/oc-11_zpsvudezuvn.png "oc theme")

## Tugas

* Lakukan instalasi OpenCart secara online.





 