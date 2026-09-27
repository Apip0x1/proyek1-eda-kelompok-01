# Analisis Eksploratif (EDA) Dataset Serangan Siber

## Kelompok 1

1. Muhammad Afif Nuromli (5027261003)
2. Muhammad Zaid Fardhan (5027261051)
3. Yang Kui Chin (5027261069)
4. Rafky Aqeela Permana (5027261127)

**Topik:** Cyber Security

## Latar Belakang

Serangan siber saat ini memiliki banyak variasi, seperti SQL Injection, XSS, CSRF, dan masih banyak lagi. Tiap serangan memiliki tingkat kerumitan tersendiri yang dapat dilihat dari seberapa panjang deskripsinya, seberapa banyak langkahnya, dan berapa alat (*tools*) yang dipakai. Dalam dataset ini, terdapat sekitar 14.000 catatan serangan yang akan dipelajari. Sebelum masuk ke analisis yang lebih kompleks, proyek ini bertujuan untuk melihat gambaran umum data menggunakan statistik deskriptif.

**Pertanyaan Analisis:**

1. Bagaimana rata-rata dan sebaran panjang deskripsi serangan (`desc_len`)?
2. Berapa rata-rata jumlah *tools* yang dipakai tiap serangan (`tools_count`), dan apakah jumlahnya bervariasi?
3. Apakah panjang langkah serangan (`steps_len`) memiliki sebaran yang simetris atau terdapat nilai yang jauh berbeda (*outlier*)?

## Sumber Dataset

* **Nama File:** `Attack_Dataset.csv`
* **Sumber/Link:** [[Kaggle]](https://www.kaggle.com/datasets/tannubarot/cybersecurity-attack-and-defence-dataset)
* **Lisensi:** [[MIT]](https://www.mit.edu/~amini/LICENSE.md)

## 3 Temuan Utama

1. **Temuan 1:** Rata-rata panjang deskripsi serangan adalah 127,57 karakter. Nilai rata-ratanya lebih besar dari nilai tengahnya (median 103), sehingga sebagian data memiliki deskripsi yang jauh lebih panjang. Penyebaran datanya juga cukup beragam, dengan simpangan baku 90,93 karakter.
2. **Temuan 2:** Rata-rata jumlah tools yang digunakan dalam satu serangan adalah sekitar 2,94 tools. Nilai ini hampir sama dengan mediannya, yaitu 3 tools, sehingga jumlah tools yang digunakan cenderung cukup stabil, biasanya sekitar 2–3 tools.
3. **Temuan 3:** Rata-rata panjang langkah serangan adalah 698,13 karakter, sedangkan mediannya 554 karakter. Perbedaan ini menunjukkan bahwa sebagian besar langkah serangan tidak terlalu panjang, tetapi ada beberapa serangan dengan langkah yang sangat panjang, bahkan mencapai 6.003 karakter.

## Struktur Folder

Folder `bagi-tugas/` sengaja dibuat sebagai ruang kerja terpisah untuk melacak riwayat pengerjaan awal dan memperlihatkan kontribusi tiap anggota secara transparan sebelum disatukan. Setelah semua bagian selesai, kode dari masing-masing anggota digabungkan ke dalam file utama `eda_kelompok_01.ipynb`.

```text
.
├── README.md
├── eda_kelompok_01.ipynb       # File notebook utama (gabungan seluruh kode)
├── bagi-tugas/
│   ├── tugas1(rafky).ipynb     # Pengerjaan bagian Rafky
│   ├── tugas2(fardhan).ipynb   # Pengerjaan bagian Fardhan
│   ├── tugas3(kui_chin).ipynb  # Pengerjaan bagian Yang Kui Chin
│   └── tugas4(Afif).ipynb      # Pengerjaan bagian Afif
└── data/
    └── Attack_Dataset.csv      # File dataset yang digunakan
```

## Cara Menjalankan Notebook

Untuk melihat dan menjalankan analisis pada repositori ini, ikuti langkah-langkah berikut.

### 1. Persiapan Environment

Pastikan **Python** sudah terinstal di komputer. Kemudian instal library yang diperlukan:

```bash
pip install pandas matplotlib seaborn jupyter
```

Jika menggunakan **JupyterLab**, dapat dijalankan dengan:

```bash
pip install jupyterlab
```

### 2. Clone Repositori

Clone repositori ke komputer menggunakan Git:

```bash
git clone <URL_REPOSITORY>
```

Kemudian masuk ke folder repositori:

```bash
cd <NAMA_FOLDER_REPOSITORY>
```

Jika tidak menggunakan Git, repositori juga dapat diunduh dalam bentuk **ZIP** kemudian diekstrak.

### 3. Pastikan Dataset Berada di Lokasi yang Benar

Pastikan file dataset berada di dalam folder `data/` dengan struktur:

```text
data/
└── Attack_Dataset.csv
```

Notebook menggunakan lokasi tersebut untuk membaca dataset. Jika file berada di lokasi lain, proses pembacaan dataset dapat mengalami error.

### 4. Buka Notebook

Buka file utama:

```text
eda_kelompok_01.ipynb
```

Notebook dapat dibuka menggunakan salah satu dari berikut:

* **Jupyter Notebook**
* **JupyterLab**
* **Visual Studio Code**
* **Google Colab**

Jika menggunakan Jupyter Notebook, jalankan:

```bash
jupyter notebook
```

Jika menggunakan JupyterLab:

```bash
jupyter lab
```

Kemudian buka file `eda_kelompok_01.ipynb`.

### 5. Jalankan Semua Cell

Setelah notebook terbuka, jalankan seluruh cell secara berurutan.

Pada Jupyter Notebook/JupyterLab dapat menggunakan menu:

```text
Kernel → Restart & Run All
```

atau tombol **Run All** pada lingkungan yang digunakan.

**Penting:** Jalankan seluruh cell sebelum melakukan *push* ke GitHub. Dengan begitu, hasil analisis, tabel, dan grafik akan tersimpan di dalam notebook sehingga dapat langsung terlihat ketika file `.ipynb` dibuka melalui GitHub.

### 6. Menjalankan Notebook di Google Colab

Notebook juga dapat dijalankan menggunakan Google Colab.

1. Buka [Google Colab](https://colab.research.google.com/).
2. Pilih **File → Open notebook**.
3. Pilih tab **GitHub** atau upload file `eda_kelompok_01.ipynb`.
4. Pastikan `Attack_Dataset.csv` tersedia di folder `data/`.
5. Jalankan seluruh cell dari awal sampai akhir.

> **Catatan:** Jika menggunakan Google Colab, pastikan path dataset sesuai dengan lokasi file di environment Colab. Jika dataset berada di repository GitHub, dataset dapat diunduh terlebih dahulu atau repository dapat di-*clone* ke environment Colab.

### 7. Menjalankan Notebook Pengerjaan Masing-Masing Anggota

Notebook pada folder `bagi-tugas/` dapat dijalankan dengan cara yang sama.

Contohnya:

```text
bagi-tugas/tugas4(Afif).ipynb
```

File-file tersebut merupakan hasil pengerjaan masing-masing anggota sebelum seluruh kode digabungkan ke dalam:

```text
eda_kelompok_01.ipynb
```
