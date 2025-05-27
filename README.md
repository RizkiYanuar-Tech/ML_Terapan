# Laporan Proyek Machine Learning - Muhammad Rizki Yanuar

## Domain Proyek

Krisis saat ini telah menyebabkan banyak lembaga keuangan di seluruh dunia mengambil langkah-langkah penting untuk menghindari risiko gagal bayar dari pelanggan yang meminjam dana. Maraknya kasus default utang konsumen mendorong para ahli untuk meninjau kembali standar dan praktik yang selama ini digunakan, guna memastikan perlindungan yang memadai bagi perusahaan dari peristiwa serupa di masa depan. [Loanification - Loan Approval Classification using Machine Learning
Algorithms]. 

Bagi setiap bank atau lembaga keuangan, pengelolaan pinjaman dan pengendalian leverage merupakan tugas krusial dalam menjaga stabilitas dan efisiensi operasional. Tanpa model bisnis pinjaman-ke-simpanan yang dirancang dengan baik, bank tidak dapat menjalankan fungsinya secara optimal. Seiring kemajuan teknologi, mekanisme pemberian dan penanganan pinjaman mengalami transformasi signifikan, salah satunya melalui penerapan pembelajaran mesin (machine learning) dan ilmu data (data science) [Optimizing Bank Loan Approval with Binary Classification Method and Deep Learning Model].

## Referensi


## Business Understanding

Dalam industri perbankan dan keuangan, salah satu tantangan terbesar adalah mengidentifikasi nasabah yang berpotensi gagal bayar (default) sejak tahap awal proses aplikasi pinjaman. Keputusan yang tidak tepat dalam pemberian kredit dapat berdampak buruk terhadap stabilitas keuangan lembaga. Oleh karena itu, diperlukan sistem prediksi yang mampu mengevaluasi risiko kredit calon peminjam secara akurat dan efisien.

Proyek ini bertujuan untuk mengembangkan model klasifikasi berbasis machine learning yang dapat memprediksi kemungkinan terjadinya gagal bayar pinjaman, dengan memanfaatkan data historis pelanggan dan berbagai atribut finansial lainnya. Model ini diharapkan dapat membantu lembaga keuangan dalam membuat keputusan pemberian pinjaman yang lebih tepat dan berbasis data.

### Problem Statements

Menjelaskan pernyataan masalah latar belakang:
- Banyak lembaga keuangan masih mengandalkan penilaian kredit konvensional yang tidak adaptif terhadap pola dan tren risiko baru.

- Keterbatasan analisis manual membuat proses penilaian kredit rentan terhadap bias dan kesalahan prediksi.

- Belum adanya sistem prediksi otomatis berbasis pembelajaran mesin yang secara akurat dapat mengklasifikasikan tingkat risiko gagal bayar dari calon peminjam.

### Goals

Menjelaskan tujuan dari pernyataan masalah:
- Mengembangkan model klasifikasi berbasis machine learning yang mampu memprediksi apakah seseorang kemungkinan akan menerima pinjaman atau tidak

### Solution statements
- Implementasi dan membandingkan model klasifikasi untuk menemukan model terbaik
- Melakukan hyperparameter tuning pada model untuk mengoptimalkan hasil klasifikasi dan meningkatkan akurasi prediksi

## Data Understanding
Paragraf awal bagian ini menjelaskan informasi mengenai data yang Anda gunakan dalam proyek. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [Loan Approval Classification](https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data).

### Variabel-variabel pada ILPD dataset adalah sebagai berikut:
- person_age: Umur orang
- person_gender: Jenis kelamin orang
- person_education: Pendidikan terakhir
- person_income: Pendapatan tahunan
- person_emp_exp: Pengalaman bekerja -tahun
- person_home_ownership: Status kepemilikan rumah
- loan_amnt: Total pinjaman yang diminta
- loan_intent: Tujuan pinjaman
- loan_int_rate: Suku bunga pinjaman
- loan_percent_income: Jumlah pinjaman sebagai persentase pendapatan tahunan
- cb_person_cred_hist_length: Lama riwayat kredit dalam tahun
- credit_score: Nilai kredit orang
- previous_loan_defaults_on_file: Indikator tunggakan pinjaman sebelumnya
- loan_status: Status persetujuan pinjaman

## Data Preparation
- Missing Value: Penanganan terhadap data yang hilang
- Duplicate: Menghapus data yang memiliki duplikasi agar tidak bias data dan tidak mengalami overfitting pada saat evaluasi model.
- Encoding: Transformasi data dengan mengubah nilai kategori ke bentuk numerik.
- Split Data: Membagi data latih dan data uji dengan proporsi 80:20

## Modeling
Pada tahap ini, beberapa algoritma klasifikasi machine learning digunakan untuk memprediksi apakah seseorang mengalami penyakit liver atau tidak.

  1. Random Forest
     kumpulan dari banyak pohon keputusan (decision trees) yang dilatih dengan data acak dan subset fitur yang berbeda. Hasil akhir ditentukan berdasarkan voting mayoritas dari semua pohon.

  Kelebihan
  
  a. Akurasi yang lebih tinggi daripada decision tree tunggal
  
  b. Lebih tahan terhadap overfitting
  
  c. Memberikan feature importance
  
  Kekurangan 
  
  a. Kurang interpretatif dibanding decision tree tunggal
  
  b. Sedikit lebih lama dalam pelatihan

  2. Gradient Boosting
     Gradient Boosting adalah sebuah teknik yang menggabungkan beberapa model yang lemah (weak model) menjadi sebuah model yang kuat.

  Kelebihan

  a. Akurasi yang tinggi: Gradient Boosting sering menghasilkan model yang akurat dan kuat, terutama ketika digunakan pada data yang kompleks dan tidak terstruktur.

  b. Kecepatan komputasi yang cepat

  Kekurangan:
  
  a. Memerlukan tuning yang cermat: Algoritma ini memerlukan tuning parameter yang cermat untuk mendapatkan model yang optimal.
  
  b. Mudah overfitting: Gradient Boosting dapat cenderung overfit pada data training jika tidak dilakukan pengaturan parameter yang baik.
  
## Evaluation
- Akurasi: Mengukur proporsi prediksi yang benar dari keseluruhan prediksi.
- Recall (Sensitivity) : Mengukur seberapa baik model dapat mendeteksi kasus positif.
- Precision : Mengukur proporsi prediksi positif yang benar-benar positif.
