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
- **Sumber/Link:** [Isi dengan link dataset, misal tautan Kaggle]
- **Lisensi:** [Isi dengan lisensi dataset, misal CC0 / MIT / Public Domain]

*(Catatan: Jika ukuran file dataset melebihi 25 MB, file tidak diunggah ke repositori GitHub. Silakan unduh melalui link di atas dan letakkan file tersebut ke dalam folder `data/` dengan nama `Attack_Dataset.csv` sebelum menjalankan notebook).*

## 3 Temuan Utama
1. **Temuan 1:** [Isi dengan kesimpulan dari analisis panjang deskripsi serangan / desc_len]
2. **Temuan 2:** [Isi dengan kesimpulan dari rata-rata dan variasi jumlah tools / tools_count]
3. **Temuan 3:** [Isi dengan kesimpulan dari sebaran dan outlier panjang langkah serangan / steps_len]

## Struktur Folder

Saat ini, pengerjaan masih dibagi per anggota sebelum digabungkan menjadi file `eda_kelompok_01.ipynb` di akhir. Struktur foldernya adalah:

```text
.
├── README.md
├── bagi-tugas/
│   ├── tugas1(rafky).ipynb     # Pengerjaan bagian/pertanyaan 1 oleh Rafky
│   ├── tugas2(fardhan).ipynb   # Pengerjaan bagian/pertanyaan 2 oleh Fardhan
│   ├── tugas3(kui_chin).ipynb  # [PLACEHOLDER - Akan diisi oleh Kui Chin]
│   └── tugas4(Afif).ipynb      # Pengerjaan bagian/pertanyaan 4 oleh Afif
└── data/
    └── Attack_Dataset.csv      # File dataset (Hanya contoh, tidak di-push jika > 25MB)
