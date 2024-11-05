# Praktikum 3

Nama: Ica Rizqiah

Kelas: TI.24.A.5

NIM: 312410554

Mata Kuliah: Bahasa Pemograman

## Penjelasan untuk code latihan 1

```python
import random
```
Modul random diimpor agar dapat menggunakan fungsi random.random(), yang berfungsi untuk menghasilkan angka acak antara 0 dan 1.

```python
n = int(input("Masukkan nilai N: "))
```
Kode ini meminta pengguna untuk memasukkan nilai integer (n). Nilai n akan menentukan berapa kali program harus menampilkan angka acak yang kurang dari 0.5.

```python
for i in range(1, n + 1):
```
Bagian ini adalah for loop yang akan menjalankan proses sebanyak n kali (dari i = 1 hingga i = n). Setiap iterasi dari loop akan menghasilkan satu angka acak yang kurang dari 0.5.

```python
 angka_acak = random.random()
    while angka_acak >= 0.5:
        angka_acak = random.random()
```
Di dalam for loop, angka_acak dihasilkan menggunakan random.random(), yang akan mengembalikan nilai acak antara 0 dan 1. Namun, jika angka acak yang dihasilkan bernilai 0.5 atau lebih, maka while loop akan terus menghasilkan angka acak baru hingga didapatkan angka yang kurang dari 0.5. Dengan demikian, angka_acak yang dihasilkan pasti selalu kurang dari 0.5.

```python
 print(f"data ke-{i} => {angka_acak}")
```
Setelah angka acak yang kurang dari 0.5 didapatkan, program akan menampilkan angka tersebut bersama dengan urutan data (data ke-i).

```python
print("Selesai")
```

Setelah semua angka acak yang kurang dari 0.5 ditampilkan sesuai jumlah yang diminta (n), program akan mencetak kata "Selesai" untuk menandakan akhir eksekusi.

## Berikut hasil code latihan 1
![foto](https://github.com/keeyyaaa/labpy03/blob/main/Screenshot%202024-11-04%20102710.png?raw=true)

## Penjelasan untuk code latihan 2

## Fungsi `hitung_keuntungan`
1. Parameter Input:

`modal_awal`: Modal awal yang diinvestasikan (dalam contoh ini, 100 juta Rp).

`laba_per_bulan`: Daftar yang berisi persentase laba yang diperoleh setiap bulan.


2. Inisialisasi:

`total_keuntungan` diinisialisasi dengan 0 untuk menyimpan total keuntungan selama periode investasi.

`laba_bulanan` adalah list kosong yang akan menyimpan laba yang diperoleh setiap bulan.


3. Perulangan:

Menggunakan loop `for` untuk iterasi melalui setiap bulan (dari 0 hingga 7, total 8 bulan).

Pada setiap iterasi:

Menghitung laba bulan tersebut dengan rumus `modal_awal` * `laba_per_bulan[bulan]`.

Menambahkan laba yang dihitung ke dalam list `laba_bulanan.`

Menambahkan laba bulan tersebut ke `total_keuntungan.`

Mencetak laba yang diperoleh untuk bulan tersebut.


4. Pengembalian Nilai:

Setelah semua bulan dihitung, fungsi mengembalikan `total_keuntungan` dan list `laba_bulanan.`


## Fungsi `main`

1. Inisialisasi Modal Awal:

Mendefinisikan `modal_awal` dengan nilai RP 100 juta .


2. Daftar Laba Per Bulan:

Mendefinisikan `laba_per_bulan` yang berisi persentase laba untuk masing-masing bulan. Dalam hal ini, laba untuk bulan 1 dan 2 adalah 0%, bulan 3 dan 4 adalah 1%, bulan 5 adalah 5%, bulan 6 adalah 3%, dan seterusnya.


3. Memanggil Fungsi hitung_keuntungan:

Memanggil fungsi `hitung_keuntungan` dengan `modal_awal` dan `laba_per_bulan` sebagai argumen.

Menyimpan hasil pengembalian fungsi ke dalam `total_keuntungan` dan `laba_bulanan.`


4. Mencetak Total Keuntungan:

Mencetak total keuntungan yang diperoleh selama 8 bulan.


## Alur Eksekusi
Saat program dijalankan, fungsi `main` akan dipanggil.

Modal awal dan laba per bulan diatur, kemudian fungsi `hitung_keuntungan` dijalankan.

Laba bulanan dihitung dan ditampilkan untuk setiap bulan, serta total keuntungan selama 8 bulan ditampilkan di akhir.

## Berikut hasil code latihan 2

![foto](https://github.com/keeyyaaa/labpy03/blob/main/Screenshot%202024-11-05%20100729.png?raw=true)

## berikut hasil code program python yang sudah di jalankan:

![foto](https://github.com/keeyyaaa/labpy03/blob/main/Screenshot%202024-11-05%20100919.png?raw=true)


# Alur algoritma latihan3: latihan3.py
Alur Algoritma Program ATM

1. Inisialisasi Saldo
   
Langkah:

Tentukan variabel 'saldo'.

Setel 'saldo' ke 1.000.000.

Tujuan: Menyimpan jumlah uang yang tersedia untuk ditarik oleh pengguna.

2. Tampilkan Pesan Selamat Datang

Langkah:

Tampilkan pesan: "Selamat datang di Mesin ATM!".

Tampilkan saldo awal: "Saldo Anda saat ini: Rp 1.000.000".

Tujuan: Memberikan informasi awal kepada pengguna tentang saldo mereka.

3. Mulai Loop Utama

Langkah:

Masuk ke dalam loop tak terbatas dengan 'while True'.

Tujuan: Memungkinkan pengguna untuk melakukan beberapa transaksi tanpa harus memulai ulang program.

4. Tampilkan Menu Pilihan

Langkah:

Tampilkan menu pilihan:

Tarik Tunai

Cek Saldo

Keluar

Tujuan: Memberikan pilihan kepada pengguna untuk melakukan tindakan yang diinginkan.

5. Minta Input dari Pengguna

Langkah:

Minta pengguna untuk memasukkan pilihan menu dengan 'input()'.

Tujuan: Mengambil keputusan dari pengguna mengenai tindakan yang ingin dilakukan.

6. Proses Berdasarkan Pilihan

Langkah:

Jika pilihan adalah '1' (Tarik Tunai):

Minta pengguna untuk memasukkan jumlah uang yang ingin ditarik.

Validasi Jumlah Penarikan:

Jika jumlah yang diminta lebih besar dari saldo:

Tampilkan pesan kesalahan: "Jumlah yang diminta melebihi saldo Anda. Silakan coba lagi."

Jika jumlah yang diminta kurang dari atau sama dengan 0:

Tampilkan pesan kesalahan: "Jumlah penarikan harus lebih dari 0. Silakan coba lagi."

Jika jumlah yang diminta valid:

Kurangi saldo dengan jumlah yang ditarik: 'saldo -= jumlah_tarik'.

Tampilkan pesan: "Anda telah menarik Rp [jumlah_tarik]. Sisa saldo Anda: Rp [saldo]."

Jika pilihan adalah '2' (Cek Saldo):

Tampilkan saldo saat ini dengan pesan: "Saldo Anda saat ini: Rp [saldo]."

Jika pilihan adalah '3' (Keluar):

Tampilkan pesan: "Terima kasih telah menggunakan Mesin ATM. Selamat tinggal!"

Keluar dari loop dengan break.

Jika pilihan tidak valid:

Tampilkan pesan kesalahan: "Pilihan tidak valid. Silakan coba lagi."

7. Kembali ke Langkah 4

Langkah:

Setelah menyelesaikan proses berdasarkan pilihan, kembali ke langkah 4 untuk menampilkan menu lagi dan meminta input pengguna.

Tujuan: Memungkinkan pengguna untuk melakukan transaksi tambahan atau keluar dari program.


# berikut code program python nya:
![foto]

