---
# A. JUDUL PROGRAM
SISTEM PENGURUTAN NAMA HEWAN MENGGUNAKAN BUBBLE SORT
---

# B. Deskripsi singkat Program "Penamaan Hewan di Kebun Binatang" 

Kodingan sederhana berbasis python yang mengurutkan nama-nama hewan kebun binatang secara A sampai Z menggunakan algoritma Bubble Sort. Program ini mengadaptasi  kode asli yang terdiri dari fungsi bubble sort ke dalam konteks penamaan hewan. Pengguna dapat memasukkan sendiri jumlah dan nama hewan yang ingin diurutkan,kemudian program akan membandingkan nama-nama tersebut satu per satu secara dan menukar posisinya jika urutannya belum benar,sehingga menghasilkan daftar nama hewan yang tersusun rapi dari huruf A hingga Z.

---

# C.SOURCE CODE
<img width="955" height="974" alt="Image" src="https://github.com/user-attachments/assets/5018bce7-2f95-4ae3-bd43-2866a2f01ff4" />
---
<img width="589" height="400" alt="Image" src="https://github.com/user-attachments/assets/db2ddfa2-dcfd-41df-86fb-53c966182bea" />
---

# PENJELASAN KODE

def tukar(arr, i, j):
= Berfungsi sebagai fungsi untuk *menukar posisi dua elemen* di dalam list. Fungsi ini menggunakan variabel sementara temp untuk menyimpan nilai sementara agar nilai asli tidak hilang saat proses penukaran berlangsung.

def bubble_sort(arr, n):
= Berfungsi sebagai fungsi *inti algoritma Bubble Sort* yang mengurutkan elemen-elemen di dalam list. Fungsi ini menggunakan dua loop bersarang untuk membandingkan setiap pasangan elemen yang bersebelahan, lalu memanggil fungsi tukar() apabila urutan elemen tersebut salah.

for i in range(n - 1):
= Berfungsi sebagai *loop luar* yang mengontrol jumlah putaran (pass). Setiap satu putaran memastikan satu elemen terbesar berpindah ke posisi akhir yang benar.

for j in range(n - i - 1):
= Berfungsi sebagai *loop dalam* yang membandingkan dua elemen yang bersebelahan. Batasnya semakin kecil setiap putaran karena elemen di bagian akhir sudah pasti terurut.

if arr[j] > arr[j + 1]:
= Berfungsi sebagai kondisi pengecekan* apakah elemen kiri lebih besar dari elemen kanan. Jika ya, maka fungsi tukar() dipanggil untuk memindahkan elemen tersebut.

def main():
= Berfungsi sebagai fungsi utama yang mengatur seluruh alur program, mulai dari menerima input jumlah dan nama hewan, memanggil fungsi bubble_sort(), hingga menampilkan hasil urutan akhir ke layar.

if __name__ == "__main__":
= Berfungsi sebagai penjaga eksekusi program, memastikan fungsi main() hanya dijalankan ketika file ini dijalankan secara langsung, bukan ketika di-import oleh file Python lain.

---

# OUTPUT KODE
<img width="728" height="685" alt="Image" src="https://github.com/user-attachments/assets/49f838a6-7e7a-4c8a-8f9e-da372ddcd4e8" /><img width="728" height="685" alt="Image" src="https://github.com/user-attachments/assets/49f838a6-7e7a-4c8a-8f9e-da372ddcd4e8" />
---
# PENJELASAN OUTPUT

---

# Output 1 - Judul Program:

Penamaan Hewan di Kebun Binatang

= Berfungsi sebagai judul program yang muncul pertama kali saat program dijalankan.

---

# Output 2 - Daftar Hewan Tersedia:

Hewan tersedia:
   1. Ayam
   2. Babi
   3. Kucing
   4. Macan
   5. Gajah
   6. Harimau
   7. Kelinci
   8. Buaya
   9. Gorila
  10. Burung
  11. Singa
  12. Rusa

= Berfungsi sebagai **daftar referensi 12 nama hewan** yang ditampilkan agar pengguna bisa memilih atau mengetik nama hewan yang ingin diurutkan.

---


# Output 3 - Input Jumlah Hewan:

Masukkan jumlah hewan yang ingin diurutkan: 6

= Berfungsi sebagai **permintaan input angka** dari pengguna. Pengguna memasukkan angka 6, artinya akan ada 6 hewan yang diurutkan.

---

---
# Output 4 - Input Nama Hewan

Hewan ke-1: ZEBRA
Hewan ke-2: GORILLA
Hewan ke-3: BURUNG
Hewan ke-4: AYAM
Hewan ke-5: SINGA
Hewan ke-6: (kosong)
Nama tidak boleh kosong, coba lagi!
Hewan ke-6: KELINCI


= Berfungsi sebagai permintaan input nama hewan satu per satu. Pada hewan ke-6 pengguna tidak mengetik apapun sehingga program menampilkan pesan "Nama tidak boleh kosong, coba lagi! lalu meminta input ulang, dan pengguna memasukkan KELINCI.

---



# Output 5 - Array Sebelum Diurutkan:  ['Zebra', 'Gorilla', 'Burung', 'Ayam', 'Singa', 'Kelinci']

= Berfungsi sebagai **tampilan kondisi awal list** sebelum Bubble Sort dijalankan, yaitu urutan sesuai yang diketik pengguna.

---

# Output 6 - Array Sesudah Diurutkan: ['Ayam Burung Gorilla Kelinci Singa Zebra']

= Berfungsi sebagai hasil akhir setelah Bubble Sort selesai bekerja, semua nama hewan sudah tersusun dari A ke Z .

---

# Output 7 - Daftar Bernomor:

Daftar hewan terurut A → Z:
  1. Ayam
  2. Burung
  3. Gorilla
  4. Kelinci
  5. Singa
  6. Zebra

= Berfungsi sebagai tampilan hasil akhir yang bernomor urut, menampilkan 6 nama hewan yang sudah terurut dengan rapi dari A hingga Z.

---

# Output 8 - Penutup:
Sorting selesai!
= Berfungsi sebagai tanda bahwa seluruh proses program telah selesai dijalankan dengan sukses.

---
