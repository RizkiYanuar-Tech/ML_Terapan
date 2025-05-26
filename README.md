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
Paragraf awal bagian ini menjelaskan informasi mengenai data yang Anda gunakan dalam proyek. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data).

Selanjutnya uraikanlah seluruh variabel atau fitur pada data. Sebagai contoh:  

### Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:
- accepts : merupakan jenis pembayaran yang diterima pada restoran tertentu.
- cuisine : merupakan jenis masakan yang disajikan pada restoran.
- dst

**Rubrik/Kriteria Tambahan (Opsional)**:
- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data atau exploratory data analysis.

## Data Preparation
Pada bagian ini Anda menerapkan dan menyebutkan teknik data preparation yang dilakukan. Teknik yang digunakan pada notebook dan laporan harus berurutan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan proses data preparation yang dilakukan
- Menjelaskan alasan mengapa diperlukan tahapan data preparation tersebut.

## Modeling
Tahapan ini membahas mengenai model machine learning yang digunakan untuk menyelesaikan permasalahan. Anda perlu menjelaskan tahapan dan parameter yang digunakan pada proses pemodelan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan kelebihan dan kekurangan dari setiap algoritma yang digunakan.
- Jika menggunakan satu algoritma pada solution statement, lakukan proses improvement terhadap model dengan hyperparameter tuning. **Jelaskan proses improvement yang dilakukan**.
- Jika menggunakan dua atau lebih algoritma pada solution statement, maka pilih model terbaik sebagai solusi. **Jelaskan mengapa memilih model tersebut sebagai model terbaik**.

## Evaluation
Pada bagian ini anda perlu menyebutkan metrik evaluasi yang digunakan. Lalu anda perlu menjelaskan hasil proyek berdasarkan metrik evaluasi yang digunakan.

Sebagai contoh, Anda memiih kasus klasifikasi dan menggunakan metrik **akurasi, precision, recall, dan F1 score**. Jelaskan mengenai beberapa hal berikut:
- Penjelasan mengenai metrik yang digunakan
- Menjelaskan hasil proyek berdasarkan metrik evaluasi

Ingatlah, metrik evaluasi yang digunakan harus sesuai dengan konteks data, problem statement, dan solusi yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan formula metrik dan bagaimana metrik tersebut bekerja.

**---Ini adalah bagian akhir laporan---**

_Catatan:_
- _Anda dapat menambahkan gambar, kode, atau tabel ke dalam laporan jika diperlukan. Temukan caranya pada contoh dokumen markdown di situs editor [Dillinger](https://dillinger.io/), [Github Guides: Mastering markdown](https://guides.github.com/features/mastering-markdown/), atau sumber lain di internet. Semangat!_
- Jika terdapat penjelasan yang harus menyertakan code snippet, tuliskan dengan sewajarnya. Tidak perlu menuliskan keseluruhan kode project, cukup bagian yang ingin dijelaskan saja.

