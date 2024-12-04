# House Price Prediction

## Domain Proyek
Proyek ini bertujuan untuk memprediksi harga properti di Melbourne dengan menggunakan fitur-fitur yang mempengaruhi nilai properti. Di tengah tingginya permintaan pasar properti, informasi mengenai harga pasar yang akurat sangat penting bagi para pembeli, penjual, dan agen properti. Model prediksi harga properti dapat membantu mereka dalam membuat keputusan yang lebih baik berdasarkan data historis dan fitur properti tertentu.

## Business Understanding
Problem Statements: Bagaimana cara memprediksi harga properti berdasarkan fitur property yang ada?
Goals: Membuat model prediksi yang dapat memberikan estimasi harga properti secara akurat. Model ini akan membantu pemangku kepentingan untuk memperkirakan nilai properti dengan lebih baik.

## Data Understanding
Dataset yang digunakan terdiri dari 13,580 baris data dengan 21 kolom yang mencakup informasi tentang properti di Melbourne. Berikut adalah beberapa variabel penting:

- Rooms: Jumlah kamar di properti
- Distance: Jarak properti dari pusat kota
- Bathroom: Jumlah kamar mandi
- Bedroom2: Jumlah kamar tidur
- Landsize: Ukuran lahan (m²)
- BuildingArea: Luas bangunan (m²)
- YearBuilt: Tahun properti dibangun
- Lattitude: Koordinat geografis properti
- Sumber data: Dataset ini dapat diunduh melalui link berikut:

https://www.kaggle.com/code/dansbecker/explore-your-data/input?select=melb_data.csv

Dalam tahap Exploratory Data Analysis (EDA), kami melakukan pemeriksaan missing values dan juga mengecek keberadaan outlier yang dapat mempengaruhi model.

## Data Preparation
Untuk persiapan data, kami menerapkan MinMaxScaler pada fitur-fitur numerik berikut:

- Rooms
- Distance
- Bathroom
- Bedroom2
- Landsize
- BuildingArea
- YearBuilt
- Lattitude

Scaling ini dilakukan untuk memastikan bahwa semua fitur memiliki rentang nilai yang seragam sehingga model dapat bekerja dengan optimal.

## Modeling
Model yang digunakan dalam proyek ini adalah Random Forest Regression. Kami menggunakan model ini secara langsung untuk menyelesaikan permasalahan tanpa metode tambahan.

## Evaluation
Untuk mengevaluasi model, metrik yang digunakan adalah R² Score. Metrik ini menunjukkan seberapa baik model dapat menjelaskan variabilitas dari data target (harga properti).

Hasil evaluasi menunjukkan bahwa model memiliki performa yang baik dalam memprediksi harga properti, dengan nilai R² Score yang cukup tinggi, menandakan model dapat memprediksi sebagian besar variabilitas dalam data harga properti.
