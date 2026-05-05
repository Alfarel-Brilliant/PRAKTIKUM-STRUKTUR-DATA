# Judul Program

Pencarian Nomor Kursi Pesawat Menggunakan Binary Search


# Deskripsi Singkat

Program ini digunakan untuk mencari nomor kursi tertentu dalam daftar nomor kursi pesawat yang sudah diurutkan secara menaik. Algoritma yang digunakan adalah Binary Search, yaitu algoritma pencarian yang bekerja dengan membagi array menjadi dua bagian pada setiap iterasi.

Binary Search memiliki kompleksitas waktu yang efisien, yaitu O(log n). Program ini meminta pengguna untuk memasukkan jumlah nomor kursi, daftar nomor kursi yang sudah diurutkan, dan nomor kursi yang ingin dicari. Jika nomor kursi ditemukan, program akan mengembalikan indeksnya. Jika tidak ditemukan, program akan memberikan pesan bahwa nomor kursi tidak ditemukan.

# SUMBER KODE
SCREENSHOT 

<img width="1186" height="1051" alt="Image" src="https://github.com/user-attachments/assets/ad101d65-837b-454f-9eef-1ebfccfec75c" />



# Output dari Source Code

Jika nomor kursi ditemukan, program akan mencetak indeks nomor kursi tersebut dalam daftar. Contohnya, jika daftar nomor kursi adalah sepuluh dua puluh tiga puluh empat puluh lima puluh dan nomor kursi yang dicari adalah tiga puluh, outputnya adalah Median dua nomor kursi tiga puluh dan Nomor kursi ditemukan pada indeks ke dua. Jika nomor kursi tidak ditemukan, program akan mencetak pesan bahwa nomor kursi tidak ditemukan. Contohnya, jika daftar nomor kursi adalah sepuluh dua puluh tiga puluh empat puluh lima puluh dan nomor kursi yang dicari adalah tiga puluh lima, outputnya adalah Median dua nomor kursi tiga puluh, Mencari nomor kursi di kanan, Median tiga nomor kursi empat puluh, Mencari nomor kursi di kiri, dan Nomor kursi tidak ditemukan.


# d. Penjelasan Logika Program Per Baris
Fungsi binary_search:
Baris l = 0 dan r = n - 1: Inisialisasi batas kiri (l) dan batas kanan (r) dari daftar.

Baris while l <= r: Loop berjalan selama batas kiri tidak melewati batas kanan.

Baris m = l + (r - l) // 2: Menghitung indeks median untuk membagi daftar menjadi dua bagian.

Baris print(f"Median: {m}, nomor kursi: {arr[m]}"): Menampilkan indeks median dan nilai pada indeks tersebut.

Baris if arr[m] == target: Mengecek apakah nilai median sama dengan nomor kursi yang dicari.

Baris elif arr[m] < target: Jika nilai median lebih kecil dari nomor kursi yang dicari, pencarian dilanjutkan ke bagian kanan daftar.

Baris else: Jika nilai median lebih besar, pencarian dilanjutkan ke bagian kiri daftar.

Baris return pos: Mengembalikan indeks nomor kursi jika ditemukan, atau -1 jika tidak ditemukan.

Fungsi main:Baris n = int(input("Masukkan jumlah nomor kursi pesawat: ")): Meminta pengguna memasukkan jumlah nomor kursi.

Baris arr = []: Inisialisasi daftar kosong untuk menyimpan nomor kursi.

Baris for i in range(n): Loop untuk meminta pengguna memasukkan nomor kursi satu per satu.

Baris arr.append(nilai): Menambahkan nomor kursi ke dalam daftar.

Baris print(f"Daftar nomor kursi: {arr}"): Menampilkan daftar nomor kursi yang telah dimasukkan.

Baris target = int(input("Masukkan nomor kursi yang ingin dicari: ")): Meminta pengguna memasukkan nomor kursi yang ingin dicari.

Baris pos = binary_search(arr, n, target): Memanggil fungsi binary_search untuk mencari nomor kursi.

Baris if pos != -1: Mengecek apakah nomor kursi ditemukan.

Baris print(f"Nomor kursi ditemukan pada indeks ke-{pos}"): Menampilkan indeks nomor kursi jika ditemukan.

Baris else: Menampilkan pesan bahwa nomor kursi tidak ditemukan.
Blok if __name__ == "__main__"::
Memastikan bahwa fungsi main hanya dijalankan jika file ini dijalankan sebagai program utama, bukan diimpor sebagai modul
