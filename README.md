# ⚽ K-Means Clustering: FIFA World Cup 2026 Player Performance

Proyek ini merupakan implementasi algoritma **K-Means Clustering**, sebuah metode *Unsupervised Machine Learning*, yang digunakan untuk mengelompokkan data berdasarkan karakteristik yang serupa. 

Pada latihan ini, model digunakan untuk menganalisis dan mengelompokkan performa pemain sepak bola berdasarkan jarak tempuh (*Distance Covered*) dan kecepatan maksimal (*Top Speed*) menggunakan dataset simulasi **FIFA World Cup 2026 Player Performance**.

---

## 🎯 Tujuan Proyek
1. Memahami konsep dasar dan cara kerja algoritma K-Means Clustering.
2. Mengimplementasikan K-Means Clustering menggunakan library `scikit-learn` pada bahasa pemrograman Python.
3. Melakukan pra-pemrosesan data numerik menggunakan teknik *Min-Max Scaling*.
4. Memvisualisasikan hasil *clustering* dan titik pusat kluster (*centroid*) dalam bentuk scatter plot.

## 📊 Dataset
Dataset yang digunakan berasal dari Kaggle: `fifa_world_cup_2026_player_performance.csv`.
Dalam proyek ini, fokus pengelompokan (*clustering*) difokuskan pada dua variabel (fitur) utama:
- **`distance_covered_km`**: Total jarak yang ditempuh pemain dalam satu pertandingan (dalam kilometer).
- **`top_speed_kmh`**: Kecepatan lari maksimal yang dicapai pemain selama pertandingan (dalam kilometer per jam).

## 🛠️ Teknologi dan Library yang Digunakan
- **Python 3**
- **Pandas**: Manipulasi dan analisis data *dataframe*.
- **NumPy**: Komputasi numerik dan operasi *array*.
- **Scikit-Learn**: Implementasi *Machine Learning* (Algoritma K-Means & Min-Max Scaler).
- **Matplotlib / Seaborn**: Visualisasi data (Scatter plot grafik persebaran data).

## 🚀 Langkah-langkah Implementasi
Proses *clustering* dalam proyek ini melalui tahapan berikut:
1. **Pengumpulan & Persiapan Data**: Memuat dataset CSV ke dalam Pandas DataFrame.
2. **Eksplorasi Data (EDA)**: Menentukan variabel yang relevan dan memvisualisasikan persebaran awal data (Scatter Plot).
3. **Normalisasi Data**: Mengubah skala data menggunakan metode *Min-Max Scaling* agar fitur dengan rentang nilai besar tidak mendominasi proses *clustering*.
4. **Pelatihan Model**: Membuat model KMeans dari library `sklearn` dengan nilai `K=3` (menghasilkan 3 kelompok profil performa pemain) dan melatihnya dengan data yang telah disesuaikan (*scaled*).
5. **Pemberian Label (Clustering)**: Menambahkan kolom `kluster` ke dataframe asli berdasarkan hasil prediksi model.
6. **Visualisasi Hasil**: Memetakan ulang titik data dan memunculkan titik pusat kluster (*centroid*) pada data yang dikembalikan ke skala aslinya (*inverse transform*).

## 📈 Hasil Visualisasi
Hasil akhir dari *script* berupa sebuah *scatter plot* interaktif yang memisahkan pemain menjadi 3 tingkatan performa mobilitas di lapangan. Titik koordinat pusat (centroid) ditandai dengan ikon 'X' berwarna merah.

---
*Proyek ini dikembangkan sebagai bagian dari latihan praktik implementasi Machine Learning sederhana menggunakan Python.*
