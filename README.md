# Laporan Proyek Machine Learning - Muhammad Rizki Yanuar

## Domain Proyek

*Liver* atau hati adalah organ yang vital bagi manusia, organ ini terletak di dalam rongga perut sebelah kanan, tepatnya di bawah diafragma. Beberapa fungsi kerja liver antara lain sebagai penawar dan penetralisir racun, mengatur sirkulasi hormon, mengatur komposisi darah yang mengadung lemak, gula, protein, dan membuat empedu, dimana zat yang membantu percernaan lemak. Penyakit *liver* merupakan suatu gangguan pada setiap fungsi *liver*, ketika *liver* kehilangan fungsi-fungsi tersebut dapat menyebabkan kerusakan yang signifikan pada tubuh [Klasifikasi Pasien Penderita Penyakit Liver dengan Pendekatan Machine Learning]. 

Hasil analisis data kematian yang dirilis oleh *British Livir Trust* pada tahun 2019 mengungkapkan bahwa penyakit hati adalah penyebab kematian terbesar di Inggris dan Wales pada rentang usia 35-49 tahun, dimana pada penelitian tersebut juga diperkirakan bahwa penyakit hati akan menggeser penyakit jantung sebagai penyebab terbesar kematian dini dalam beberapa tahun mendatang, permalasahan yang biasanya terjadi pada penyakit *liver* adalah mengenali penyakit tersebut sejak dini, bahkan ketika penyakiy tersebut sudah menyebar. Padahal pemeriksaan kesehatan secara berkala diperlukan untuk mendeteksi penyakit *liver* sejak dini, sehingga dapat di tangani lebih cepat dan tingkat kematian karena penyakit *liver* dapat menurun [Analisis Pengaruh Komposisi Data Training dan Data Testing].

## Referensi


## Business Understanding

Penyakit hati adalah penyebab kematian terbesar di Inggris dan Wales pada rentang usia 35-49 tahun, dan penyakit hati akan menggeser penyakit jantung sebagai penyebab terbesar kematian dini dalam beberapa tahun mendatang. Pemeriksaan kesehatan secara berkala diperlukan untuk mendeteksi penyakit liver sejak dini.

Proyek ini bertujuan Mengembangkan model klasifikasi berbasis machine learning yang mampu memprediksi apakah seseorang kemungkinan besar memerlukan perawatan kesehatan mental atau tidak, berdasarkan atribut survei yang diberikan.

### Problem Statements

Menjelaskan pernyataan masalah latar belakang:
- Banyak individu dengan potensi gangguan kesehatan mental tidak terdeteksi secara dini, baik karena keterbatasan akses terhadap layanan psikologis maupun kurangnya kesadaran individu terhadap kondisi mereka sendiri.

### Goals

Menjelaskan tujuan dari pernyataan masalah:
- Mengembangkan model klasifikasi berbasis machine learning yang mampu memprediksi apakah seseorang kemungkinan mengalami penyakit liver atau tidak

### Solution statements
- Implementasi dan membandingkan model klasifikasi untuk menemukan model terbaik
- Melakukan hyperparameter tuning pada model untuk mengoptimalkan hasil klasifikasi dan meningkatkan akurasi prediksi

## Data Understanding
Paragraf awal bagian ini menjelaskan informasi mengenai data yang Anda gunakan dalam proyek. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [Indian Liver Dataset](https://www.kaggle.com/datasets/uciml/indian-liver-patient-records). 

### Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:
- Age of the patient: Umur pasien yang check liver.
- Gender of the patient: Jenis kelamin pasien.
- Total Bilirubin: Pigmen kuning yang ditemukan pada darah, empedu dan urin
- Direct Bilirubin: Bilirubin yang diolah oleh hati dan menjadi mudah larut dalam air
- Alkaline Phosphotase: Enzim di seluruh tubuh untuk mineralisasi tulang dan produksi empedu, Kadar ALP tinggi mengindikasikan gangguan fungsi hati
- Alamine Aminostransferase: Enzim yang sebagian besar ada di hati, peningkatan kadar Alamine menunjukkan adanya kerusakan atau cedera pada sel hati
- Aspartate Aminotransferase: Enzim yang berperan dalam metabolisme asam amino, peningkatan kadar AST dalam darah mengindikasikan adanya kerusakan sel hati, penyakit hati
- Total Proteins: Jumlah protein yang terdapat dalam darah
- Albumin: Protein yang dihasilkan hati untuk mensintesis sel hati
- Albumin and Globulin Ratio: Perbandingan kadar albumin dan globulin dalam darah
- Dataset: Label pasien terkena *liver* atau tidak

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
