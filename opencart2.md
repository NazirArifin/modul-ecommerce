# OpenCart 2. Bahasa & Mata Uang

## Ubah Bahasa Indonesia

* Unduh extension bahasa Indonesia [Paket Modul Bahasa Indonesia OpenCart versi 2](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=21907&filter_search=indonesia&filter_category_id=2&filter_license=0).

* Untuk dapat menginstal ekstensi bahasa, jika Anda memasang dan menggunakan OpenCart secara online maka Anda harus mengeset pengaturan FTP di menu __System__ > __Setting__. Edit toko Anda lalu lengkapi pengaturan FTP yang ada di tab FTP.

* Gunakan menu __Extensions__ > __Extension Installer__ untuk meletakkan file yang dibutuhkan ke server.

### Copy Manual
* Jika Anda memasang dan menggunakan OpenCart secara offline maka Anda harus meletakkan secara manual file yang ada di paket installer yang telah Anda download.

* Folder (beserta file didalamnya) diletakkan pada path berikut:
```
admin/language/id-id
catalog/language/id-id
```

* Selanjutnya gunakan menu __System__ > __Localisation__ > __Languages__ lalu tekan tombol [+] diatas halaman untuk menambahkan bahasa Indonesia ke sistem.

*  Isikan data berikut di inputan yang tersedia:
```
Language Name: Indonesia
Code: id-id
Locale: id_ID.UTF-8,id_ID,id-id,indonesia
Status: Enabled
Sort Order: 1
```
* Untuk mengeset bahasa Indonesia menjadi bahasa default maka Anda dapat menggunakan menu __System__ > __Settings__ lalu edit toko Anda dan ubah di tab __Local__. Anda dapat mengubah pengaturan Language dan Administration Language ke bahasa Indonesia.

* Jika sukses maka di halaman depan toko Anda akan terdapat pilihan menu bahasa yang dapat diganti-ganti oleh pengunjung.


## Ubah Mata Uang / _Currency_

* Anda dapat menggunakan menu __System__ > __Localisation__ > __Currencies__ lalu menekan tombol [+] dibagian atas halaman.

* Isikan data berikut di inputan yang tersedia:
```
Currency Title: Rupiah
Code: IDR
Symbol Left: Rp.
Symbol Right: 
Decimal Places: 0
Values: 1
Status: Enabled
```

* Untuk mengeset mata uang Rupiah menjadi default maka Anda dapat menggunakan menu yang sama dengan saat mengeset bahasa.

