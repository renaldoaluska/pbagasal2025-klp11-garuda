# Analisis Sentimen, POS, dan NER Maskapai Garuda Indonesia pada Artikel Berita

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg) ![Framework](https://img.shields.io/badge/Framework-Selenium-green.svg) ![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)

Repositori ini berisi kode dan sumber daya untuk proyek **Analisis Sentimen, Part-of-Speech (POS) Tagging, dan Named Entity Recognition (NER)** terhadap maskapai Garuda Indonesia berdasarkan data artikel berita daring.

---

## 📄 Informasi Proyek

Proyek ini merupakan tugas akhir untuk mata kuliah **Pengolahan Bahasa Alami (A)** pada Departemen Sistem Informasi, Institut Teknologi Sepuluh Nopember (ITS) untuk Semester Gasal 2025.

**Anggota Kelompok 11:**
* Jason Ho (5026221005)
* Alfa Renaldo Aluska (5026221144)

## 🎯 Latar Belakang

Di era digital, persepsi publik terhadap sebuah korporasi seperti Garuda Indonesia sangat dipengaruhi oleh pemberitaan di media daring. Berbeda dari media sosial yang subjektif, artikel berita memiliki struktur bahasa yang lebih formal dan kredibilitas yang lebih tinggi. Penelitian ini bertujuan untuk menganalisis secara komprehensif bagaimana Garuda Indonesia direpresentasikan di media massa melalui tiga pendekatan utama: analisis sentimen, identifikasi entitas (NER), dan penandaan kelas kata (POS tagging).

## ⚙️ Metodologi Penelitian

Alur kerja penelitian ini dibagi menjadi tiga tahap utama sesuai dengan yang dijelaskan dalam laporan:

1.  **Akuisisi Data:**
    * Mengumpulkan data artikel berita dari Google News dengan kata kunci "Garuda Indonesia".
    * Proses *scraping* dilakukan secara otomatis menggunakan **Python** dengan pustaka **Selenium** untuk mengekstraksi judul, tautan, tanggal terbit, dan nama portal.
    * Konten lengkap dari setiap artikel kemudian diunduh berdasarkan tautan yang telah dikumpulkan.

2.  **Pra-pemrosesan & EDA:**
    * Membersihkan data teks dari artikel berbahasa Inggris.
    * Melakukan standarisasi teks melalui *lowercasing* (mengubah ke huruf kecil).
    * Menghapus kata-kata umum yang tidak signifikan (*stopwords removal*).
    * Mengubah kata ke bentuk dasarnya melalui proses *lemmatization* atau *stemming*.
    * Melakukan Analisis Data Eksploratif (EDA) untuk memahami distribusi data.

3.  **Analisis:**
    * Menerapkan **TF-IDF** untuk ekstraksi fitur dan mengidentifikasi kata-kata penting.
    * Melakukan **Analisis Sentimen** untuk mengklasifikasikan artikel ke dalam sentimen positif, negatif, atau netral.
    * Menerapkan **POS Tagging** dan **NER** untuk mendapatkan wawasan gramatikal dan mengidentifikasi entitas seperti nama orang, organisasi, dan lokasi.

## 📂 Struktur Repositori

Repositori ini diatur dengan struktur sebagai berikut untuk kemudahan navigasi dan replikasi:
.
├── data/
│   ├── raw/
│   │   └── link_berita_garudaindonesia.csv  (Data mentah hasil scraping)
│   └── processed/
│       └── garuda_news_preprocessed.csv   (Data bersih siap analisis)
├── notebooks/
│   ├── 01_Data_Acquisition.ipynb          (Notebook untuk scraping data)
│   ├── 02_Preprocessing_and_EDA.ipynb     (Notebook untuk pembersihan dan EDA)
│   └── 03_Analysis_and_Modeling.ipynb     (Notebook untuk TF-IDF, Sentimen, POS, NER)
├── report/
│   └── 2025-1_Klp-11_Paper.pdf            (Laporan akhir proyek)
├── requirements.txt                       (Daftar pustaka Python yang dibutuhkan)
└── README.md                              (Anda sedang membacanya)


## 🚀 Cara Menjalankan

Untuk mereplikasi hasil dari penelitian ini, ikuti langkah-langkah berikut:

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/renaldoaluska/pbagasal2025-klp11-garuda.git](https://github.com/renaldoaluska/pbagasal2025-klp11-garuda.git)
    cd pbagasal2025-klp11-garuda
    ```

2.  **Buat Lingkungan Virtual (Opsional tapi Direkomendasikan)**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Untuk Windows: venv\Scripts\activate
    ```

3.  **Instal Dependensi**
    Pastikan Anda memiliki file `requirements.txt` yang berisi semua pustaka yang digunakan, lalu jalankan:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Jalankan Notebooks**
    Buka dan jalankan Jupyter Notebooks di dalam direktori `/notebooks` secara berurutan:
    -   `01_Data_Acquisition.ipynb`
    -   `02_Preprocessing_and_EDA.ipynb`
    -   `03_Analysis_and_Modeling.ipynb`

## 📊 Hasil dan Pembahasan

Hasil analisis mendalam, temuan utama, visualisasi data, dan kesimpulan disajikan secara lengkap dalam laporan akhir proyek. Silakan merujuk ke dokumen:
[**`report/2025-1_Klp-11_Paper.pdf`**](./report/2025-1_Klp-11_Paper.pdf)

---
