# UTS Machine Learning - Jalur C (Clustering)

## Identitas

- **Nama**: Ferdinandus Mantur
- **NIM**: 2301010389
- **Kelas**: XX
- **Mata Kuliah**: Machine Learning
- **Dosen**: Dr. I Gede Totok Suryawan, S.Kom., M.T.
- **Tanggal**: 26 November 2026

## Judul Proyek

**Segmentasi Kabupaten/Kota di Indonesia Berdasarkan Indeks Pembangunan Manusia (IPM) Menggunakan K-Means Clustering**

## Deskripsi Singkat

Proyek ini melakukan segmentasi 514 kabupaten/kota di Indonesia berdasarkan 5 indikator pembangunan manusia (AHH, RLS, HLS, Pengeluaran per Kapita, dan IPM) menggunakan algoritma K-Means Clustering. Hasil clustering membagi daerah menjadi 2 kelompok: **Daerah Maju** (28.79%) dan **Daerah Berkembang** (71.21%), dengan Silhouette Score 0.3877.

## Struktur Repository

UTS-ML-2301010389-Ferdinandus Mantur/
├── README.md
├── notebook/
│ └── UTS ML_2301010389 Ferdinandus Mantur.ipynb
├── data/
│ └── IPM-Indonesia-2023.xlsx
└── reports/
├── grafik_utama.png
└── slide_presentasi.pdf

## Dataset

- **Nama**: IPM-Indonesia-2023
- **Sumber**: Kaggle (Sumber asli: Badan Pusat Statistik / Satu Data Indonesia)
- **Link**: https://www.kaggle.com/datasets/sherlydwipuspita/ipm-indonesia-2023
- **Jumlah Data**: 514 baris (kabupaten/kota), 5 fitur numerik
- **Lisensi**: Data publik BPS, bebas digunakan untuk penelitian

## Cara Menjalankan Notebook

1. Buka Google Colab: https://colab.research.google.com/
2. Upload file `notebook/UTS_ML_2301010389_Ferdinandus Mantur.ipynb`
3. Upload file `data/IPM-Indonesia-2023.xlsx` ke Colab
4. Jalankan **Runtime → Run all**
5. Semua output akan tampil secara otomatis

## Hasil Utama

- **Algoritma**: K-Means dengan k=2, StandardScaler
- **Silhouette Score**: 0.3877 (CUKUP)
- **PCA Variansi**: 89.42% (PCA1: 73.34%, PCA2: 16.08%)
- **Cluster 0 (Daerah Maju)**: 148 kabupaten/kota (28.79%)
- **Cluster 1 (Daerah Berkembang)**: 366 kabupaten/kota (71.21%)

## Pernyataan Penggunaan AI

Saya, Ferdinandus Mantur (NIM: 2301010389), menyatakan bahwa dalam pengerjaan proyek UTS Machine Learning ini, saya menggunakan asisten AI sebagai berikut:

**Alat AI yang Digunakan**: Qwen (asisten AI berbasis large language model)

**Bagian yang Dibantu AI**:

1. **Penjelasan Konsep**: AI membantu menjelaskan konsep K-Means Clustering, Silhouette Score, PCA, dan metode pra-pemrosesan (clipping outlier, StandardScaler) agar saya memahami teori di balik kode.
2. **Struktur Notebook**: AI membantu menyusun struktur notebook sesuai alur CRISP-DM dan rubrik penilaian UTS.
3. **Debugging**: AI membantu mengidentifikasi dan memperbaiki error (misal: NameError karena variabel tidak terdefinisi, inkonsistensi antara output dan interpretasi).
4. **Template Kode**: AI menyediakan template kode untuk visualisasi (histogram, heatmap, boxplot, PCA 2D, silhouette plot) dan pemodelan K-Means, yang kemudian saya modifikasi dan sesuaikan dengan dataset saya.
5. **Interpretasi Hasil**: AI membantu merumuskan interpretasi bisnis dari hasil clustering dan rekomendasi strategis, yang kemudian saya validasi dengan pemahaman saya sendiri.

**Bagian yang Saya Kerjakan Sendiri**:

1. **Pemilihan Dataset**: Saya memilih dataset IPM-Indonesia-2023 dari Kaggle berdasarkan minat pribadi terhadap isu pembangunan daerah.
2. **Registrasi ELSA**: Saya mendaftarkan dataset secara mandiri.
3. **Modifikasi Kode**: Semua kode yang disediakan AI saya baca, pahami, dan modifikasi sesuai kebutuhan (misal: menyesuaikan nama kolom, mengubah parameter visualisasi, memperbaiki logika).
4. **Pengambilan Keputusan**: Keputusan akhir (k = 2, penamaan cluster "Daerah Maju" vs "Daerah Berkembang", rekomendasi strategi) saya buat sendiri berdasarkan pemahaman terhadap output dan konteks bisnis.
5. **Presentasi**: Saya akan mempresentasikan hasil proyek ini secara mandiri dan mampu menjelaskan serta mengubah kode saat tanya jawab.

**Verifikasi Hasil**: Saya telah memeriksa semua output kode, memverifikasi angka yang dilaporkan, dan memastikan interpretasi sesuai dengan hasil analisis. Tidak ada hasil yang langsung saya copy-paste tanpa pemahaman.

**Tanggal**: 25 November 2026
