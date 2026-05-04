---
# A. JUDUL PROGRAM
SISTEM PENGURUTAN NAMA HEWAN MENGGUNAKAN BUBBLE SORT
---

# B. Deskripsi singkat Program "Penamaan Hewan di Kebun Binatang" 

Kodingan sederhana berbasis python yang mengurutkan nama-nama hewan kebun binatang secara A sampai Z menggunakan algoritma Bubble Sort. Program ini mengadaptasi  kode asli yang terdiri dari fungsi bubble sort ke dalam konteks penamaan hewan. Pengguna dapat memasukkan sendiri jumlah dan nama hewan yang ingin diurutkan,kemudian program akan membandingkan nama-nama tersebut satu per satu secara dan menukar posisinya jika urutannya belum benar,sehingga menghasilkan daftar nama hewan yang tersusun rapi dari huruf A hingga Z.

---

# C.SOURCE CODE

<img width="657" height="719" alt="Image" src="https://github.com/user-attachments/assets/9bd9406c-ae88-4c27-a733-5473621475d4" />


# PENJELASAN KODE

1. def tukar(arr, i, j): = Berfungsi sebagai fungsi untuk menukar posisi dua elemen di dalam list.

2. temp = arr[i] = Berfungsi untuk menyimpan nilai elemen pada indeks i ke dalam variabel sementara bernama temp.

3. arr[i] = arr[j] = Berfungsi untuk mengisi posisi indeks i dengan nilai yang ada di indeks j.

4. arr[j] = temp = Berfungsi untuk mengisi posisi indeks j dengan nilai yang sebelumnya disimpan di variabel temp, sehingga proses penukaran selesai.

5. def bubble_sort(arr, n): = Berfungsi sebagai fungsi inti algoritma Bubble Sort yang mengurutkan elemen-elemen di dalam list.

6. for i in range(n - 1): = Berfungsi sebagai perulangan luar yang berjalan sebanyak n-1 kali, mewakili setiap putaran (pass) dari proses pengurutan.

7. for j in range(n - i - 1): = Berfungsi sebagai perulangan dalam yang membandingkan elemen-elemen berdekatan, dengan batas yang semakin mengecil setiap putaran karena elemen terbesar sudah berada di posisi akhir.

8. if arr[j] > arr[j + 1]: = Berfungsi untuk memeriksa apakah elemen pada posisi j lebih besar dari elemen pada posisi j+1, jika iya maka akan dilakukan penukaran posisi.

9. tukar(arr, j, j + 1) = Berfungsi untuk memanggil fungsi tukar guna menukar posisi elemen pada indeks j dengan elemen pada indeks j+1.

10. def main(): = Berfungsi sebagai fungsi utama yang menjalankan keseluruhan program dari awal hingga akhir.

11. try: = Berfungsi untuk memulai blok percobaan yang akan menangkap kesalahan jika input yang dimasukkan pengguna tidak sesuai.

12. n = int(input("Masukkan jumlah hewan di kebun binatang: ")) = Berfungsi untuk meminta pengguna memasukkan jumlah hewan dan mengubah input tersebut menjadi bilangan bulat yang disimpan di variabel n.

13. except ValueError: = Berfungsi untuk menangkap kesalahan apabila pengguna memasukkan input yang bukan angka.

14. print("Input tidak valid!") = Berfungsi untuk menampilkan pesan kesalahan kepada pengguna bahwa input yang dimasukkan tidak valid.

15. return = Berfungsi untuk menghentikan eksekusi fungsi main secara langsung saat terjadi kesalahan input.

16. arr = [] = Berfungsi untuk membuat sebuah list kosong yang nantinya akan diisi dengan nama-nama hewan.

17. print("Masukkan nama hewan:") = Berfungsi untuk menampilkan perintah kepada pengguna agar memasukkan nama hewan satu per satu.

18. for i in range(n): = Berfungsi sebagai perulangan yang berjalan sebanyak n kali sesuai jumlah hewan yang diinputkan sebelumnya.

19. nama = input() = Berfungsi untuk menerima input nama hewan dari pengguna dan menyimpannya ke dalam variabel nama.

20. arr.append(nama) = Berfungsi untuk menambahkan nama hewan yang baru dimasukkan ke dalam list arr.

21. print(f"Daftar hewan sebelum diurutkan: {arr}") = Berfungsi untuk menampilkan seluruh isi list sebelum proses pengurutan dilakukan.

22. bubble_sort(arr, n) = Berfungsi untuk memanggil fungsi bubble_sort guna mengurutkan elemen-elemen di dalam list arr.

23. print("Daftar hewan setelah diurutkan (Bubble Sort):", end=" ") = Berfungsi untuk menampilkan teks judul hasil pengurutan tanpa berpindah ke baris baru.

24. for i in range(n): = Berfungsi sebagai perulangan untuk mencetak setiap elemen yang sudah diurutkan satu per satu.

25. print(arr[i], end=" ") = Berfungsi untuk mencetak nama hewan pada indeks i dengan spasi sebagai pemisah antar nama tanpa berpindah baris.

26. print() = Berfungsi untuk mencetak baris kosong sehingga output berpindah ke baris baru setelah semua nama hewan ditampilkan.

27. if __name__ == "__main__": = Berfungsi untuk memastikan bahwa fungsi main hanya akan dijalankan jika file ini dieksekusi secara langsung, bukan ketika diimpor sebagai modul oleh file lain.

28. main() = Berfungsi untuk memanggil dan menjalankan fungsi main sehingga seluruh program dapat berjalan.

---

# OUTPUT KODE
<img width="812" height="237" alt="Image" src="https://github.com/user-attachments/assets/10bf477a-1d14-4e6f-9a44-1ffcf528142a" />

---

# PENJELASAN OUTPUT


1. Input Data:

Program meminta pengguna untuk memasukkan jumlah hewan yang ada di kebun binatang.

Kemudian, pengguna memasukkan nama-nama hewan satu per satu sebanyak 7 hewan:

Ayam

Bebek

Buaya

Zebra

Harimau

Macan

Panda


2. Daftar hewan sebelum diurutkan:

Setelah nama-nama hewan dimasukkan, program menampilkan daftar hewan sebelum dilakukan pengurutan:

[Ayam, Bebek, Buaya, Zebra, Harimau,Macan,Panda.]



3. Daftar hewan setelah diurutkan:

Program kemudian mengurutkan daftar nama hewan menggunakan algoritma Bubble Sort. Algoritma ini mengurutkan data secara bertahap, memindahkan elemen yang lebih besar ke posisi yang lebih tinggi.

Hasil pengurutan dengan algoritma Bubble Sort menghasilkan daftar:

[Ayam,Bebek, Buaya, Harimau, Macan, Panda ,Zebra.]

Dan output terakhir selesai

---
