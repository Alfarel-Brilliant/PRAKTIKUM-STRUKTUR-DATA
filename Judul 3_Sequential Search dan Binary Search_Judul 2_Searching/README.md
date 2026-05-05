# Judul Program

Pencarian Nomor Kursi Pesawat Menggunakan Binary Search


# Deskripsi Singkat

Program ini digunakan untuk mencari nomor kursi tertentu dalam daftar nomor kursi pesawat yang sudah diurutkan secara menaik. Algoritma yang digunakan adalah Binary Search, yaitu algoritma pencarian yang bekerja dengan membagi array menjadi dua bagian pada setiap iterasi.

Binary Search memiliki kompleksitas waktu yang efisien, yaitu O(log n). Program ini meminta pengguna untuk memasukkan jumlah nomor kursi, daftar nomor kursi yang sudah diurutkan, dan nomor kursi yang ingin dicari. Jika nomor kursi ditemukan, program akan mengembalikan indeksnya. Jika tidak ditemukan, program akan memberikan pesan bahwa nomor kursi tidak ditemukan.

# SUMBER KODE
SCREENSHOT 

<img width="1186" height="1051" alt="Image" src="https://github.com/user-attachments/assets/ad101d65-837b-454f-9eef-1ebfccfec75c" />

# Penjelasan Logika Per Baris

def binary_search(arr, n, target):
Fungsi ini digunakan untuk mencari posisi nomor kursi tertentu (target) dalam daftar nomor kursi (arr) yang sudah diurutkan dengan panjang n. Binary search bekerja dengan membagi daftar menjadi dua bagian secara terus-menerus hingga menemukan nomor kursi yang dicari atau memastikan bahwa nomor tersebut tidak ada  .

l = 0 dan r = n - 1
Inisialisasi batas pencarian. l adalah batas kiri (indeks awal), dan r adalah batas kanan (indeks akhir). Pencarian dimulai dari seluruh daftar .

pos = -1
Variabel pos disiapkan untuk menyimpan posisi hasil pencarian. Nilai awalnya -1, yang berarti nomor kursi belum ditemukan.

while l <= r:
Perulangan dilakukan selama batas kiri (l) tidak melewati batas kanan (r). Ini memastikan bahwa masih ada bagian daftar yang bisa diperiksa .

m = l + (r - l) // 2
Menghitung indeks tengah m untuk membagi daftar menjadi dua bagian. Indeks tengah dihitung dengan rumus ini untuk menghindari overflow pada daftar yang sangat besar.

print(f"Median: {m}, nomor kursi: {arr[m]}")
Menampilkan indeks tengah (m) dan nilai nomor kursi di posisi tersebut. Ini membantu pengguna memahami proses pencarian.

if arr[m] == target:
Jika nomor kursi di tengah sama dengan nomor yang dicari (target), maka nomor kursi ditemukan .

pos = m dan break
Simpan posisi nomor kursi yang ditemukan ke dalam variabel pos dan hentikan pencarian .

elif arr[m] < target:
Jika nomor kursi di tengah lebih kecil dari nomor yang dicari, maka pencarian dilanjutkan di bagian kanan daftar .

print("Mencari nomor kursi di kanan") dan l = m + 1
Menampilkan informasi bahwa pencarian dilanjutkan ke kanan, dan batas kiri (l) digeser ke kanan dari indeks tengah.

else:
Jika nomor kursi di tengah lebih besar dari nomor yang dicari, maka pencarian dilanjutkan di bagian kiri daftar .

print("Mencari nomor kursi di kiri") dan r = m - 1
Menampilkan informasi bahwa pencarian dilanjutkan ke kiri, dan batas kanan (r) digeser ke kiri dari indeks tengah.

return pos
Mengembalikan posisi hasil pencarian. Jika nomor kursi ditemukan, posisi indeksnya dikembalikan. Jika tidak ditemukan, -1 dikembalikan.

def main():
Fungsi utama program yang mengatur input dan output. Fungsi ini meminta pengguna memasukkan jumlah nomor kursi, daftar nomor kursi, dan nomor kursi yang ingin dicari.

try: dan n = int(input("Masukkan jumlah nomor kursi pesawat: "))
Meminta input jumlah nomor kursi. Jika input bukan angka, program akan menampilkan pesan error dan keluar dari fungsi.

arr = [] dan print("Masukkan nomor kursi (urut menaik):")
Membuat daftar kosong untuk menyimpan nomor kursi dan memberikan instruksi kepada pengguna untuk memasukkan nomor kursi secara berurutan.

for i in range(n):
Melakukan perulangan sebanyak n kali untuk meminta input nomor kursi dari pengguna.

while True: dan try:
Memastikan bahwa input nomor kursi valid berupa angka. Jika input tidak valid, pengguna diminta untuk mengulanginya.

arr.append(nilai)
Menambahkan nomor kursi yang valid ke dalam daftar.

print(f"Daftar nomor kursi: {arr}")
Menampilkan daftar nomor kursi yang sudah dimasukkan oleh pengguna.

while True: dan try:
Meminta input nomor kursi yang ingin dicari. Jika input tidak valid, pengguna diminta untuk mengulanginya.

pos = binary_search(arr, n, target)
Memanggil fungsi binary_search untuk mencari posisi nomor kursi yang dimasukkan pengguna .

if pos != -1:
Jika posisi nomor kursi ditemukan (bukan -1), program menampilkan indeksnya.

else:
Jika posisi nomor kursi tidak ditemukan, program menampilkan pesan bahwa nomor kursi tidak ada.

if __name__ == "__main__":
Memastikan bahwa fungsi main() hanya dijalankan jika file ini dieksekusi langsung, bukan diimpor sebagai modul.

main()
Menjalankan fungsi utama program untuk memulai proses pencarian nomor kursi.

# Output dari Source Code




