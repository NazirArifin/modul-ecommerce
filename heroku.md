# Hosting PHP di [HEROKU](https://www.heroku.com)

## Apakah heroku.com

> Heroku is a cloud platform that lets companies build, deliver, monitor and scale apps — we're the fastest way to go from idea to URL, bypassing all those infrastructure headaches.

## Membuat Aplikasi di heroku.com

- Pastikan Anda sudah terdaftar di heroku.com dengan mengakses halaman [daftar](https://signup.heroku.com/). Isi inputan dan daftar dan _CREATE FREE ACCOUNT_.

- Install [heroku toolbelt](https://devcenter.heroku.com/articles/heroku-cli) yang mana berisi heroku CLI, dan git. Sesuaikan dengan sistem operasi serta arsitektur komputer Anda.

- Setelah heroku toolbelt ter-_install_, buka __command prompt__ dan ketikkan perintah berikut:

```sh
heroku login
```
- Masukkan email dan password yang Anda gunakan saat mendaftar di heroku.

- Install [composer](https://getcomposer.org/) untuk manajemen _dependencies_ di PHP. Heroku akan mengenali aplikasi PHP dengan mendeteksi keberadaan file __composer.json__.

- Pastikan bahwa kebutuhan sistem (PHP, Composer dan Git) telah terpenuhi dengan menggunakan perintah berikut:

```sh
$ php -v
```

```sh
$ composer -v
```

```sh
$ git --version
```

- Buat folder baru untuk aplikasi yang akan dikerjakan lalu ketikkan perintah:

```sh
$ git init
```

- Buat file _composer.json_ dengan menggunakan perintah:

```sh
$ composer init
```
- Ikuti perintah yang muncul saat perintah diatas dihasilkan. Untuk _dependency_ dan _dev dependency_ dapat diabaikan (jawab __no__). Pastikan bagian yang memasukkan folder __vendor__ ke _.gitignore_ Anda jawab __yes__.

- Buat file `index.php` dengan mengetikkan perintah

```sh
$ touch index.php
```

- Edit file `index.php` dengan teks editor kesayanganmu dan masukkan kode berikut: (hanya untuk contoh)

```php
<?php

echo 'Hello World';

?>
```

- Pastikan terdapat tiga file yaitu __composer.json__, __.gitignore__, dan __index.php__ di dalam folder kerja.

- Ketikkan perintah untuk membuat aplikasi di heroku:

```sh
$ heroku create
```

- Heroku akan meng-_generate_ nama acak sebagai lokasi / _url_ aplikasi Anda sekaligus memasukkan git remote ke dalam git.

- Lakukan update git terhadap beberapa file yang kita buat dengan perintah berikut:

```sh
$ git add .
$ git commit -am "tambah file index, composer"
```
- Lakukan push untuk mengupload file _local_ ke aplikasi  di heroku dengan perintah:

```sh
$ git push heroku master
```

- Tunggu beberapa saat, heroku sedang men-_deploy_ aplikasi dan untuk melihat hasilnya aplikasi yang kita buat di _browser_ maka Anda dapat mengetikkan:

```sh
$ heroku open
```  
