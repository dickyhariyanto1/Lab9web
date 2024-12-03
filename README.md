# Lab9web
|Nama|NIM|Kelas|Matkul|
|-----|-----|-----|-----|
|Dicky Jadi Hariyanto|312310374|TI 23A.4|Pemog Web|

|Modularisasi Menggunakan Require|

Modularisasi menggunakan require adalah teknik dalam pemrograman PHP yang digunakan untuk menggabungkan skrip PHP atau teks dari file lain dengan skrip PHP yang memanggilnya.
Jenis modularisasi di dalam php antara lain ; require() digunakan ketika file yang disertakan sangat penting untuk kelangsungan program, include() digunakan jika file tidak kritis untuk kelangsungan program, require_once() digunakan untuk mencegah penyertaan file yang sama lebih dari sekali (menghindari error seperti deklarasi ulang fungsi atau variabel), include_once() digunakan untuk mencegah penyertaan file yang sama lebih dari sekali, seperti require_once, tetapi tidak menghentikan eksekusi jika file tidak ditemukan.
Pada praktikum ini adalah hasil pengimplementasian dari modul praktikum 8.
 ![gambar1](https://github.com/user-attachments/assets/85f78f17-9a64-43fa-a949-4a9aa0225078)
diatas ini adalah table *data_barang* dari database yang telah dibuat.
 ![gambar1-1](https://github.com/user-attachments/assets/5e6cfcb8-3bbf-4f14-92d4-d43c12377fee)
dan diatas ini adalah isi data/value dari table *data_barang* 

**Berikut adalah screenshot beserta penjelasan dari kode yang telah dibuat**

 ![gambar home](https://github.com/user-attachments/assets/c505acd1-9769-4e73-a912-49dcb68e46c6)
terdapat tulisan *Koneksi Berhasil!* yang berarti program berhasil membuat koneksi ke database menggunakan mysqli_connect(). (*kode dapat dilihat pada koneksi.php*) 

 ![gambar menu barang](https://github.com/user-attachments/assets/ff8cb694-fd37-4e64-9f4e-146fd0f86976)
pada halaman home ini kita menggunakan fungsi require() untuk memanggil *header.php* yang akan menampilkan bagian header halaman, *tambah.php* akan menampilkan form untuk menambah data, *footer.php* untuk menampilkan bagian footer halaman. (*kode bisa dilihat pada home.php, header.php, tambah.php, footer.php*)

 ![menu barang setelah di isi](https://github.com/user-attachments/assets/b43c54e1-77ef-4951-9741-409e3245d43c)
pada kode PHP ini kita dapat mengubah data barang dalam sebuah database, termasuk gambar, melalui HTML. pada kode *error_reporting(E_ALL)*, digunakan untuk Mengaktifkan pelaporan semua jenis kesalahan PHP, termasuk peringatan dan notifikasi, yang sangat berguna selama pengembangan. *include_once 'koneksi.php';* akan menyertakan file koneksi.php, yang berisi kode untuk koneksi ke database. pada Query SQL dibuat untuk memperbarui data barang berdasarkan id_barang yang diterima dari form. (*kode dapat dilihat pada ubah.php*) 

 ![pp](https://github.com/user-attachments/assets/799ebc18-5d8b-4e8e-9750-2e81b727620f)
pada halaman kontak ini kita menggunakan *require('header.php');* dan *require('footer.php');* untuk menampilkan header dan footer yang telah kita buat, untuk selebihnya kita membuat form kontak dan informasi kontak seperti biasa. (*kode dapat dilihat pada kontak.php*)
