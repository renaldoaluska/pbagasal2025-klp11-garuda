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

Repositori ini diatur dengan struktur sebagai berikut untuk kemudahan navigasi dan replikasi.

---
