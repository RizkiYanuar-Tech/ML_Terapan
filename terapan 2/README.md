# Laporan Proyek Machine Learning - Muhammad Rizki Yanuar

## Domain Proyek
Perpustakaan memiliki ruang rak yang terbatas, tetapi masih memiliki cukup buku yang cukup banyak hingga pemilihan buku menjadi sulit dan memakan waktu, tetapi jumlah buku dan pengguna tidak cukup untuk menghasilkan teknik kolaboratif tradisional yang mengandalkan data dalam jumlah besar[].

Apalagi Penggunaan internet untuk mencari informasi cenderung meningkat, terutama peningkatann pada pencarian buku di perpustakan atau penggunaan perpustakaan untuk mencari buku. Sehingga dikembangkan dalam sistem perpustakaan untuk meningkatkan efektivitas pencarian informasi untuk memenuhi kepuasaan pengguna, salah satu teknik yang digunakan adalah sistem rekomendasi[]. 

Sistem rekomendasi buku dirancang dengan mempertimbangkan kecepatan perubahan waktu. Dengan menggunakan catatan peminjaman perpustakaan, dimana sistem bisa menyarankan kepada pustakawan buku apa yang harus dibeli, atapun untuk pengguna dapat membantu untuk menyarankan untuk membeli atau membaca buku yang sesuai untuknya dengan mempertimbangkan berbagai kriteria seperti preferensi, biaya dan fitur lain[].

## Referensi


## Business Understanding

Perpustakaan saat ini menghadapi tantangan dalam pengelolaan koleksi buku yang besar dengan ruang rak yang terbatas dan jumlah pengguna yang tidak terlalu banyak. Di sisi lain, pengguna semakin bergantung pada teknologi dan internet untuk mencari informasi, termasuk pencarian buku. Untuk meningkatkan layanan dan efisiensi pencarian informasi di perpustakaan, dibutuhkan sistem cerdas yang mampu memberikan rekomendasi buku secara personal.

Penerapan sistem rekomendasi buku dapat membantu pengguna menemukan buku yang relevan tanpa harus mencari secara manual, serta membantu pustakawan dalam pengambilan keputusan terkait pembelian atau penambahan koleksi berdasarkan preferensi dan riwayat peminjaman. Hal ini akan meningkatkan kepuasan pengguna dan efisiensi operasional perpustakaan.

### Problem Statements

Menjelaskan pernyataan masalah latar belakang:
- Sistem pencarian buku masih bersifat umum dan belum mempertimbangkan preferensi pengguna secara personal seperti genre favorit, biaya, dan minat sebelumnya.

- Pustakawan kesulitan menentukan buku apa yang sebaiknya dibeli atau dipertahankan dalam koleksi karena tidak adanya sistem yang menganalisis riwayat peminjaman dan tren minat pengguna.

### Goals
Menjelaskan tujuan dari pernyataan masalah:
- Meningkatkan efisiensi pencarian buku di perpustakaan dengan menyediakan sistem rekomendasi yang relevan dan personal.

- Meningkatkan kepuasan pengguna melalui saran buku yang sesuai dengan preferensi, minat, atau riwayat bacaan mereka.

### Solution statements
- Dikembangkan sistem rekomendasi buku berbasis data rating dan preferensi pengguna.

- Menyertakan modul analitik untuk membantu pustakawan dalam menentukan buku yang paling relevan untuk ditambahkan ke koleksi, berdasarkan pola minat pengguna dan tren peminjaman.

## Data Understanding
Dataset yang saya gunakan berasal dari kaggle: [goodbooks-10k](https://www.kaggle.com/datasets/zygmunt/goodbooks-10k?select=books.csv). Dataset ini berisikan 6 file csv yaitu:
- book_tags.csv
- books.csv
- ratings.csv
- sample_book.xml
- tags.csv
- to_read.csv

Dari 6 file csv tersebut, saya hanya menggunakan  file 4 csv yaitu:
- books.csv = Metadata buku
- ratings.csv = rating user terhadap buku
- tags.csv = tags nama buku
- book_tags.csv = tag pada buku

### Variabel-variabel pada Loan Approval Classification dataset adalah sebagai berikut:
books.csv
- book_id
- average_rating
- authors
- title
- language_code
- original_publication_year

ratings.csv
- book_id
- user_id
- rating

tags.csv
- tag_id
- tag_name

book_tags.csv
- goodreads_book_id
- tag_id
- count

## Data Preparation
- Rename Columns: Merubah nama kolom untuk memudahkan dalam penggabungan data
- Data Integration: Menggabungkan data menjadi 1 DataFrame
- Drop Columns: Menghapus kolom yang tidak digunakan
- Handling Missing Values: Mengatasi nilai kosong pada data
- Handling Duplicated: Menghapus data duplikat
- Content Integration: Menggabungkan metadata menjadi 1 kolom

## Modeling
Pada tahap ini menggunakan metode hybrid recommendation yang menggabungkan collaborative filtering dan content based filtering

  1. Collaborative Filtering
  Memanfaatkan data histori pengguna untuk memberikan rekomendasi berdasarkan kesamaan dengan histori pengguna lain

  Kelebihan
  
  a. Tidak membutuhkan data tambahan seperti deskripsi produk atau genre film
  
  b. Teknik ini dapat menemukan hubungan atau kesamaan yang tidak langsung terlihat antara pengguna dan item.
  
  Kekurangan 
  
  a. (Cold Start) Sulit memberikan rekomendasi kepada pengguna baru atau item baru yang belum memiliki data peringkat yang cukup
  
  b. (Sparsity) Sebagian besar pengguna hanya berinteraksi dengan sebagian kecil item, sehingga data menjadi jarang dan rekomendasi menjadi kurang akurat.
  
## Evaluation

- RMSE: Akurasi dalam memprediksi rating yang akan diberikan pengguna pada buku

- Recall@K: Mengukur dari kumpulan buku, berapa buku yang cocok untuk pengguna dan terdapat dalam daftar rekomendasi

- Precision@K: Dari buku yang dijadikan rekomendasi, berapa buku yang relevan dengan user

- NDCG@K: Mengukur kualitas rekomendasi berdasarkan urutan item yang direkomendasikan memiliki bobot tinggi pada item relevan berada di posisi atas.

## Hasil
RMSE yang dihasilkan pada data latih dan data uji[Collaborative Filtering RMSE]

##Kesimpulan

