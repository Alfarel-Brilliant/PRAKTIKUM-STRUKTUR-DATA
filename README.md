# SISTEM PEMESANAN TIKET ACARA (LINKED LIST)

# A. Judul program
SISTEM PEMESANAN TIKET ACARA MENGGUNAKAN LINKED LIST

# B. DESKRIPSI SINGKAT
Program ini adalah sistem pemesanan tiket acara yang menggunakan struktur data linked list untuk mengelola pemesanan. Setiap pemesanan tiket disimpan dalam node yang menyimpan data seperti nama pemesan, nama acara, jumlah tiket, kategori tiket, dan total harga. Pengguna dapat menambah pemesanan tiket baru dengan memilih kategori tiket (VIP, Reguler, atau Ekonomi), menentukan jumlah tiket, dan melihat konfirmasi pemesanan. Pemesanan akan ditambahkan ke akhir daftar, dan jika diperlukan, pengguna dapat membatalkan atau mencari pemesanan berdasarkan nama.Dengan menggunakan linked list, program ini memudahkan pengelolaan data pemesanan, seperti penambahan dan penghapusan, serta menjaga daftar tetap terstruktur dengan efisien.
# SOURCE CODE 
SCREENSHOT SOURCE CODE
<img width="1402" height="876" alt="Image" src="https://github.com/user-attachments/assets/db6bd623-cd59-4bba-91c1-ea4bbed2b6b1" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------
<img width="1180" height="858" alt="Image" src="https://github.com/user-attachments/assets/871626dc-5854-413a-a37c-4847ed2b4d8c" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------
<img width="1308" height="715" alt="Image" src="https://github.com/user-attachments/assets/c6327c21-96e9-417f-a1cc-225657009346" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------
<img width="1321" height="782" alt="Image" src="https://github.com/user-attachments/assets/16e5dd97-5de0-4e98-82aa-90cb67f28ea8" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1384" height="841" alt="Image" src="https://github.com/user-attachments/assets/7daa4cd7-8e48-4dd9-a523-db102775b96d" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1093" height="383" alt="Image" src="https://github.com/user-attachments/assets/9228f501-6654-4ab0-928f-10577abbcf0b" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

# PENJELASAN KODE

1.Class Node: Menyimpan data pemesanan tiket (tiket) dan referensi ke node berikutnya (next).

2.Class LinkedList: Menangani daftar pemesanan tiket menggunakan linked list, dengan operasi untuk menambah, menampilkan, memproses, membatalkan, dan mencari pemesanan tiket.

3.Fungsi tambah_pemesanan: Menambah pemesanan tiket baru ke dalam daftar (linked list).

4.Fungsi tampilkan_pemesanan: Menampilkan seluruh pemesanan tiket yang ada dalam daftar.

5.Fungsi proses_pemesanan: Memproses pemesanan pertama dalam daftar dan menghapusnya setelah dikirimkan.

6.Fungsi batalkan_pemesanan: Membatalkan pemesanan berdasarkan nama pemesan.

7.Fungsi cari_pemesanan: Mencari pemesanan berdasarkan nama pemesan dan menampilkan detailnya.

8.Harga Kategori Tiket: Menyimpan harga tiket untuk kategori VIP, Reguler, dan Ekonomi.

9.Fungsi input_pemesanan: Mengambil input dari pengguna untuk membuat pemesanan tiket.

10.Fungsi menu: Menampilkan menu utama untuk memilih aksi yang akan dilakukan (tambah, tampilkan, proses, cari, batalkan, keluar).

11.Fungsi main: Mengelola alur utama program dengan menerima input dari pengguna untuk memilih menu dan menjalankan aksi yang sesuai.

# D.OUTPUT PROGRAM
<img width="901" height="375" alt="Image" src="https://github.com/user-attachments/assets/f71d6e86-5014-4c24-a98c-e24fc9900592" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="968" height="388" alt="Image" src="https://github.com/user-attachments/assets/984fd721-86cb-4375-881b-a6c767613f18" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="940" height="366" alt="Image" src="https://github.com/user-attachments/assets/047724b4-6dbb-4f67-9887-71d70a459982" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1014" height="270" alt="Image" src="https://github.com/user-attachments/assets/84dca532-0038-45a8-9ff0-406f74d406d0" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="991" height="430" alt="Image" src="https://github.com/user-attachments/assets/127638f2-d219-4b41-867b-5b5008618d10" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="993" height="274" alt="Image" src="https://github.com/user-attachments/assets/aa3e5062-d049-4b95-bc17-c994589fedc9" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="628" height="286" alt="Image" src="https://github.com/user-attachments/assets/dfb5877e-d6e0-4a7e-8007-4492090d1add" />
--------------------------------------------------------------------------------------------------------------------------------------------------------------
# PENJELASAN SINGKAT OUTPUT

*Tampilan Menu Utama:Program menampilkan menu sistem pemesanan tiket acara yang berisi pilihan tambah pemesanan, tampilkan data, proses pemesanan, cari, batalkan,      dan keluar.

1. Menu 1 Tambah pemesanan tiket
User memilih menu 1 lalu mengisi nama pemesan ALFAREL, nama acara KONSER JASTIN BIBIR, memilih kategori VIP, dan jumlah tiket 2. Setelah itu sistem menampilkan pesan bahwa pemesanan berhasil ditambahkan.

2. Menu 2 Tampilkan semua pemesanan
Program menampilkan daftar pemesanan yang sudah masuk, berisi data pemesan, nama acara, jumlah tiket, kategori tiket, dan total harga yaitu Rp20.000.000.

3. Menu 3 Proses pemesanan pertama
Sistem memproses data pemesanan pertama atas nama ALFAREL dan menampilkan pesan bahwa tiket berhasil diproses serta dikirimkan.

4. Menu 4 Cari pemesanan
User mencari nama ALFAREL, lalu sistem menampilkan detail data pemesanan yang ditemukan.

5. Menu 5 Batalkan pemesanan
User memilih menu pembatalan dan memasukkan nama ALFAREL. Sistem menampilkan pesan bahwa pemesanan berhasil dibatalkan.

6. Menu 6 Keluar
Program menampilkan ucapan terima kasih, lalu sistem selesai dijalankan.

E. LINK YOUTUBE
