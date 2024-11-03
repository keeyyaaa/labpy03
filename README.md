# Praktikum 3

Nama: Ica Rizqiah

Kelas: TI.24.A.5

NIM: 312410554

Mata Kuliah: Bahasa Pemograman

# Penjelasan untuk code latihan 1

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

Kode di atas merupakan program Python yang meminta pengguna untuk memasukkan jumlah angka acak (n) yang ingin ditampilkan, di mana setiap angka acak tersebut harus kurang dari 0.5. Berikut adalah penjelasan setiap bagian dari kode tersebut:

