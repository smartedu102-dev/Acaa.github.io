## Implementasi Struktur Perulangan

Program ini dibuat dengan menerapkan beberapa jenis struktur perulangan yang dipelajari pada mata kuliah Algoritma dan Pemrograman. Setiap jenis perulangan digunakan pada fitur yang berbeda sesuai dengan kebutuhan program.

---

### 1. Perulangan For

Perulangan `for` digunakan ketika jumlah pengulangan sudah diketahui sebelumnya. Pada program ini, perulangan `for` digunakan untuk proses input data mahasiswa, menampilkan data mahasiswa, dan menghitung statistik nilai.

Contoh implementasi:

```python
for i in range(jumlah):
    nama.append(input("Nama : "))
    nim.append(input("NIM : "))
    nilai.append(float(input("Nilai : ")))
```

Penjelasan:

- Variabel `jumlah` berisi banyaknya data yang akan dimasukkan.
- Perulangan akan berjalan sesuai jumlah data yang diinput pengguna.
- Setiap iterasi digunakan untuk menyimpan data mahasiswa ke dalam array.

---

### 2. Perulangan While

Perulangan `while` digunakan ketika jumlah pengulangan belum diketahui secara pasti dan bergantung pada suatu kondisi.

Pada program ini, `while` digunakan untuk melakukan pencarian data mahasiswa berdasarkan NIM.

Contoh implementasi:

```python
i = 0

while i < len(nim):
    if nim[i] == cari:
        ditemukan = True
        break
    i += 1
```

Penjelasan:

- Program akan memeriksa setiap data NIM satu per satu.
- Jika NIM yang dicari ditemukan, proses pencarian dihentikan menggunakan `break`.
- Jika belum ditemukan, indeks akan bertambah sampai seluruh data diperiksa.

---

### 3. Perulangan Do-While (Simulasi)

Bahasa Python tidak memiliki struktur `do-while` secara langsung. Oleh karena itu, implementasinya dilakukan menggunakan `while True`.

Contoh implementasi:

```python
while True:
    jawab = input("Yakin keluar? (y/t): ")

    if jawab == "y" or jawab == "t":
        break
```

Penjelasan:

- Program akan selalu menjalankan blok perintah minimal satu kali.
- Pengguna diminta memasukkan pilihan yang valid.
- Jika pengguna memasukkan `y` atau `t`, maka perulangan dihentikan.
- Konsep ini sama dengan mekanisme `do-while` pada bahasa pemrograman lain.

---

### 4. Nested Loop (Perulangan Bersarang)

Nested Loop adalah perulangan yang berada di dalam perulangan lainnya. Pada program ini digunakan untuk membuat pola segitiga bintang.

Contoh implementasi:

```python
for i in range(1, tinggi + 1):
    for j in range(i):
        print("*", end=" ")
    print()
```

Penjelasan:

- Perulangan luar (`for i`) menentukan jumlah baris.
- Perulangan dalam (`for j`) menentukan jumlah bintang pada setiap baris.
- Semakin besar nilai `i`, semakin banyak bintang yang ditampilkan.

Output:

```text
*
* *
* * *
* * * *
* * * * *
```

---

## Kesimpulan

Berdasarkan hasil implementasi program, seluruh jenis perulangan yang dipersyaratkan pada tugas berhasil diterapkan, yaitu:

| Jenis Perulangan | Implementasi |
|-----------------|--------------|
| For | Input dan menampilkan data |
| While | Pencarian data mahasiswa |
| Do-While | Konfirmasi keluar program |
| Nested Loop | Pembuatan pola bintang |

Penggunaan berbagai jenis perulangan tersebut membantu program berjalan lebih efektif dan sesuai dengan kebutuhan masing-masing proses.
