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
- **Nama File:** `Attack_Dataset.csv`
- **Sumber/Link:** [[Kaggle]](https://www.kaggle.com/datasets/tannubarot/cybersecurity-attack-and-defence-dataset)
- **Lisensi:** [[MIT]](https://www.mit.edu/~amini/LICENSE.md)

## 3 Temuan Utama
1. **Temuan 1:** Rata-rata panjang deskripsi serangan adalah 127,57 karakter. Nilai rata-ratanya lebih besar dari nilai tengahnya (median 103), sehingga sebagian data memiliki deskripsi yang jauh lebih panjang. Penyebaran datanya juga cukup beragam, dengan simpangan baku 90,93 karakter.
2. **Temuan 2:** Rata-rata jumlah tools yang digunakan dalam satu serangan adalah sekitar 2,94 tools. Nilai ini hampir sama dengan mediannya, yaitu 3 tools, sehingga jumlah tools yang digunakan cenderung cukup stabil, biasanya sekitar 2–3 tools.
3. **Temuan 3:** Rata-rata panjang langkah serangan adalah 698,13 karakter, sedangkan mediannya 554 karakter. Perbedaan ini menunjukkan bahwa sebagian besar langkah serangan tidak terlalu panjang, tetapi ada beberapa serangan dengan langkah yang sangat panjang, bahkan mencapai 6.003 karakter.

## Struktur Folder

Folder `bagi-tugas/` sengaja dibuat untuk melacak riwayat pengerjaan dan memperlihatkan kontribusi masing-masing anggota secara transparan
```text
.
├── README.md
├── bagi-tugas/
│   ├── tugas1(rafky).ipynb     # Pengerjaan bagian Rafky
│   ├── tugas2(fardhan).ipynb   # Pengerjaan bagian Fardhan
│   ├── tugas3(kui_chin).ipynb  # Pengerjaan bagian Yang Kui Chin
│   └── tugas4(Afif).ipynb      # Pengerjaan bagian Afif
└── data/
    └── Attack_Dataset.csv      
