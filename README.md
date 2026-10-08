# Pertemuan 06 Nested Loop Python

## Identitas

- **Nama:** Madiha
- **NIM:** 2225250119
- **Kelas:** 3E
- **Mata Kuliah:** Algoritma dan Pemrograman

## Tujuan

Repository ini dibuat untuk mendokumentasikan hasil latihan dan tugas pada Pertemuan 06 mengenai *Nested Loop* dalam Python. Tujuan pembelajaran ini adalah memahami penggunaan perulangan bersarang, membuat pola menggunakan perulangan, melakukan akumulasi nilai, serta menghitung jumlah pasangan dan kondisi tertentu.

## Daftar Program

| No. | Nama File | Deskripsi |
|---:|---|---|
| 1 | `01_pasangan_indeks.py` | Menampilkan pasangan indeks menggunakan nested loop. |
| 2 | `02_pola_segitiga.py` | Membuat pola segitiga menggunakan simbol bintang. |
| 3 | `03_jumlah_per_baris.py` | Menghitung jumlah nilai pada setiap baris. |
| 4 | `04_hitung_pasangan.py` | Menghitung banyaknya pasangan berdasarkan nilai input. |
| 5 | `tabel_perkalian_dan_statistik.py` | Membuat tabel perkalian dan menghitung statistik hasilnya. |

## Cara Menjalankan Program

Pastikan Python sudah terpasang pada komputer. Buka terminal di folder repository, kemudian jalankan program menggunakan perintah berikut:

```bash
python latihan/01_pasangan_indeks.py
python latihan/02_pola_segitiga.py
python latihan/03_jumlah_per_baris.py
python latihan/04_hitung_pasangan.py
python tugas/tabel_perkalian_dan_statistik.py
```

## Algoritma Tugas 3

Program `tabel_perkalian_dan_statistik.py` digunakan untuk membuat tabel perkalian sekaligus menghitung jumlah hasil perkalian dan banyaknya hasil yang bernilai genap.

Algoritma program:

1. Meminta pengguna memasukkan nilai `n`.
2. Menginisialisasi `total_semua` dan `count_genap` dengan nilai awal 0 sebelum loop luar.
3. Menggunakan loop luar (`i`) untuk menentukan baris tabel perkalian.
4. Menginisialisasi `total_baris` dengan nilai 0 pada setiap baris.
5. Menggunakan loop dalam (`j`) untuk menghitung hasil perkalian pada setiap kolom.
6. Menghitung hasil perkalian dengan rumus `hasil = i * j`.
7. Menambahkan hasil perkalian ke `total_baris` dan `total_semua`.
8. Menggunakan kondisi `if` untuk memeriksa apakah hasil perkalian merupakan bilangan genap. Jika ya, `count_genap` ditambah 1.
9. Menampilkan jumlah hasil perkalian pada setiap baris.
10. Menampilkan total seluruh hasil dan banyaknya hasil perkalian yang genap.

### Konsep yang Digunakan

- **Nested loop:** Perulangan di dalam perulangan untuk menghasilkan tabel perkalian.
- **Akumulator `total_baris`:** Menjumlahkan hasil perkalian pada setiap baris.
- **Akumulator `total_semua`:** Menjumlahkan seluruh hasil perkalian dalam tabel.
- **Counter `count_genap`:** Menghitung banyaknya hasil perkalian yang bernilai genap.
- **Seleksi `if`:** Memeriksa kondisi bilangan genap menggunakan operator modulus (`%`).

## Hasil Pengujian

Pengujian dilakukan dengan menggunakan tiga nilai input, yaitu `n = 1`, `n = 2`, dan `n = 3`.

| Input `n` | Banyak Pasangan | Total Seluruh Hasil | Banyak Hasil Genap | Status |
|---:|---:|---:|---:|---|
| 1 | 1 | 1 | 0 | Berhasil |
| 2 | 4 | 9 | 3 | Berhasil |
| 3 | 9 | 36 | 5 | Berhasil |

Berdasarkan hasil pengujian, program berhasil menghasilkan jumlah seluruh hasil perkalian dan menghitung banyaknya hasil genap sesuai dengan nilai input.

### Contoh Hasil Tabel Perkalian untuk `n = 3`

| `i \ j` | 1 | 2 | 3 | Jumlah Baris |
|---:|---:|---:|---:|---:|
| 1 | 1 | 2 | 3 | 6 |
| 2 | 2 | 4 | 6 | 12 |
| 3 | 3 | 6 | 9 | 18 |
| **Total** | | | | **36** |

Dari tabel tersebut, diperoleh total seluruh hasil perkalian sebesar 36 dan banyaknya hasil perkalian genap sebanyak 5.

## Analisis Efisiensi

Jika nilai input adalah `n`, loop luar berjalan sebanyak `n` kali dan loop dalam juga berjalan sebanyak `n` kali untuk setiap iterasi
