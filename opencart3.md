# OpenCart 3. Metode Pembayaran & Pengiriman

## Menambah Payment Gateway

Payment Gateway merupakan metode pembayaran yang ditawarkan ke calon pembeli toko online yang kita buat. Berikut ini adalah salah satu cara untuk menambahkan payment gateway ke Opencart:

* Unduh modul untuk bank BCA, BNI dan BRI [disini](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=27777&filter_search=bca&filter_category_id=3&filter_license=0). Anda akan melihat tiga folder di dalamnya yaitu:

== foto 1

* Untuk setiap folder terdapat masing-masing folder __admin__ dan __catalog__. Ekstrak dua folder tersebut ke direktori instalasi Opencart Anda yang juga memiliki folder __admin__ dan __catalog__. Jika toko Anda online maka Anda dapat menggunakan FTP untuk meletakkan file yang telah diekstrak.

* Agar foto bank dapat muncul disaat proses pembayaran maka Anda perlu mengedit file __catalog/language/_id-id_/extension/payment/bank_bca.php__ baris ke-3 menjadi:

```php
$_['text_title']       = '<img src="http://localhost/catalog/view/image/bca.png" alt="Bank BCA" title="Bank BCA" /></a>';
```
dimana bagian `http://localhost` Anda ubah sesuai dengan alamat website Anda. Untuk bank BNI dan BRI dapat Anda lakukan cara sama dengan nama file __bank_bni.php__ dan __bank_bri.php__ pada folder yang sama.

* Sekarang di halaman Administrator, akses menu __Ekstensions__ > __Ekstensions__, lalu di bagian _Choose the extension type_ pilih bagian __Payments__. Anda akan melihat di tabel payment method terdapat logo bank BCA, BNI dan BRI.

* Untuk masing-masing bank tekan tombol [+] untuk menginstall modul tersebut. Jika sudah maka Anda dapat mengedit pengaturan dari masing-masing bank seperti gambar berikut:

== foto 2

* Jika sudah terisi tekan tombol __Simpan__ dipojok kanan atas. Lakukan pengaturan lain untuk bank BNI dan BRI sesuai dan pastikan statusnya Enabled.


== foto 3

### Tugas
* Tambahkan modul untuk bank Mandiri

## Menambah Shipping Method

Shipping method adalah metode yang ditawarkan oleh toko Anda untuk mengirimkan barang yang telah dibeli ke pembeli berdasarkan alamat yang telah diberikan. Berikut ini adalah salah satu cara untuk menambahkan shipping ke Opencart:

* Unduh modul untuk pengiriman menggunakan JNE, Tiki dan POS Indonesia [disini](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=28004&filter_search=jne&filter_category_id=4&filter_license=0). Setelah itu ekstrak folder yang ada didalamnya yaitu __admin__, __catalog__ dan __system__. Jika toko Anda online maka Anda dapat menggunakan aplikasi FTP untuk meletakkan file yang telah diekstrak.

* Kita perlu menambahkan Geozone ke Opencart dengan menggunakan menu __System__ > __Localisation__ > __Geo Zones__ lalu tekan tombol [+] dipojok kanan atas untuk menambahkan Geo Zone baru.

* Bagian Geo Zone Name diisi dengan: `JNE Reg` dan Description diisi dengan `JNE Reg shipping`, di bagian Country pilih `Indonesia` dengan Zone `all zones` lalu tekan tombol __Save__ dipojok kanan atas. 

== foto 4

* Untuk kurir lain seperti Tiki dan POS dapat dilakukan penambahan dengan cara yang sama.

* Untuk menambahkan shipping method menggunakan menu __Extensions__ > __Extensions__ dan di bagian Choose the extension type pilih __Shipping__. Cari __Indonesia Shipping__ di tabel lalu Install dengan menekan tombol [+]. Setelah itu edit Indonesia Shipping. Dibagian General Statusnya diubah __Enabled__, di __JNE Reg__ bagian Rates diisi dengan `5:10000,7:12000,10:15000,15:20000` sebagai contoh dengan format __(Berat:Harga,Berat:Harga)__. Pastikan __Status__ diisi dengan __Enabled__.

== foto 5

### Tugas
* Tambahkan shipping method untuk kurir POS Indonesia



 
  

