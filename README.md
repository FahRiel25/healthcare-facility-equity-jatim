<div align="center">

# Analisis dan Klasifikasi Tingkat Kecukupan Fasilitas Kesehatan di Kabupaten/Kota Provinsi Jawa Timur Menggunakan Machine Learning

[![SDG 3](https://img.shields.io/badge/SDG-3%3A%20Good%20Health%20and%20Well--Being-4C9F38)](https://sdgs.un.org/goals/goal3)
[![Target 3.8](https://img.shields.io/badge/Target-3.8%3A%20Universal%20Health%20Coverage-2B6CB0)](https://sdgs.un.org/goals/goal3)

</div>

Repositori ini memuat berkas proposal, perancangan pembelajaran mesin, serta dokumentasi eksperimen model analisis dan klasifikasi tingkat kecukupan fasilitas kesehatan (rumah sakit, puskesmas, klinik) dan tenaga kesehatan (dokter, perawat, bidan) terhadap jumlah penduduk pada kabupaten/kota di Provinsi Jawa Timur. Seluruh pengembangan disusun mengacu pada siklus **L-M-O-P** (*Learning Problem, Model Design, Optimization, Predict & Evaluate*).

---

## IDENTITAS KELOMPOK

- **Anggota Kelompok:**
  1. Muhsyam Fahriel Septiansyah — `244311021`
  2. Dila Alif Regita — `244311010`
- **Program Studi:** D4 Teknologi Rekayasa Perangkat Lunak
- **Mata Kuliah:** Data Science
- **Dosen Pengampu:** Gus Nanang Syaifuddiin, S.Kom., M.Kom.
- **Tahun Akademik:** 2026/2027

---

## DAFTAR PUSTAKA DAN BERKAS DOKUMEN

Struktur direktori dokumentasi pada folder `docs/` dirinci sebagai berikut:

- [docs/Formulir Pengajuan Ide]()
  Formulir pengajuan ide Checkpoint 1 (Lampiran B) yang memuat rumusan target klasifikasi multikelas, sumber dataset BPS Jawa Timur, rencana tiga model, pertimbangan etika, dan referensi awal.
- [docs/Laporan_Proyek_ML_LMOP.md](docs/Laporan_Proyek_ML_LMOP.md)
  Draf utama laporan komprehensif yang mencakup kerangka kerja siklus hidup proyek dari tahap perumusan masalah hingga evaluasi model.
- [docs/Proposal Proyek Data Science_9.docx](docs/Proposal%20Proyek%20Data%20Science_9.docx)
  Dokumen laporan proposal proyek Data Science (Bab 1 hingga Bab 3).

---

## RINGKASAN PROYEK

Proyek ini bertujuan mengidentifikasi variasi dan ketimpangan ketersediaan fasilitas serta tenaga kesehatan antar kabupaten/kota di Provinsi Jawa Timur dengan mempertimbangkan rasio jumlah penduduk yang dilayani, guna mendukung pencapaian **SDG 3 (Target 3.8)**. Tugas pembelajaran mesin dirumuskan sebagai **klasifikasi multikelas** (*Rendah*, *Sedang*, dan *Tinggi*) menggunakan tiga pendekatan model secara bertahap:

- **Baseline Model**
  *Decision Tree Classifier* sebagai pembanding dasar yang mudah diinterpretasikan melalui aturan percabangan fitur indikator kesehatan dan kependudukan.
- **Advanced Model**
  *Random Forest Classifier* dengan pendekatan *ensemble* untuk menangkap hubungan non-linear serta interaksi antarfitur fasilitas kesehatan, tenaga medis, dan populasi wilayah secara lebih stabil.
- **Deep Learning Model**
  *Multilayer Perceptron (MLP)* untuk data tabular dengan minimal dua *hidden layer*, fungsi aktivasi ReLU, regularisasi *Dropout*, serta *output layer* beraktivasi *Softmax* untuk menghasilkan probabilitas tiga kelas tingkat kecukupan.
