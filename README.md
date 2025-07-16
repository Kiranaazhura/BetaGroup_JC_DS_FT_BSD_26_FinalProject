# **Prediksi Harga Mobil Bekas di Arab Saudi pada Platform Syarah.com Menggunakan Machine Learning**

## 1. Gambaran Proyek
Proyek ini bertujuan untuk mengembangkan sistem prediksi harga mobil bekas di Arab Saudi menggunakan pendekatan machine learning. Dengan menganalisis berbagai fitur kendaraan seperti merek, tahun pembuatan, jarak tempuh, kapasitas mesin, dan kondisi kendaraan, sistem ini akan memberikan estimasi harga yang lebih objektif dan akurat. Tujuan akhir dari proyek ini adalah untuk membantu pengguna Syarah.com, baik pembeli maupun penjual, dalam membuat keputusan transaksi yang lebih cerdas dan efisien.

### Tujuan Utama:
- Membangun model machine learning yang mampu memprediksi harga mobil bekas secara akurat dan andal untuk pasar otomotif Arab Saudi, dengan memanfaatkan data historis kendaraan.
- Mengidentifikasi serta menganalisis fitur-fitur utama yang memengaruhi harga mobil bekas, seperti tahun produksi, jarak tempuh, merek, kapasitas mesin, dan atribut kendaraan lainnya, guna memahami kontribusinya terhadap nilai pasar kendaraan.
- Merancang sistem prediksi harga berbasis machine learning yang dapat diintegrasikan ke dalam platform Syarah.com, dengan tujuan untuk:
    + Membantu penjual dalam menetapkan harga yang kompetitif dan sesuai pasar.
    + Memberikan acuan harga yang objektif bagi pembeli untuk pengambilan keputusan.
    + Mendukung efisiensi operasional dan meningkatkan potensi margin keuntungan bagi perusahaan melalui proses evaluasi harga yang lebih cepat dan konsisten.

## 2. Sumber Data
- `UsedCarsSA_Unclean_EN.csv` yang didapat dari dataset [Saudi Arabia Used Cars Dataset](https://www.kaggle.com/datasets/turkibintalib/saudi-arabia-used-cars-dataset) yang berisi data penjualan mobil bekas di Arab Saudi dengan berbagai fitur seperti tipe mobil, merek mobil, tahun pembuatan, jarak tempuh, bahan bakar, warna, transmisi, harga mobil, dan lainnya.

## 3. Teknologi yang Digunakan
- Bahasa Pemrograman
    + Python - Bahasa pemrograman utama untuk pemrosesan data dan machine learning.
- Library & Framework
    + Pandas - Untuk manipulasi data dan analisis data.
    + Seaborn dan matplotlib.pyplot - Untuk visualisasi data.
    + Sklearn - Untuk berbagai teknik machine learning dan pemrosesan data, termasuk scaling, encoding, imputation, dan model evaluation.
    + Statsmodels - Untuk interpretasi model statistik.
    + Catboost - Untuk model gradient boosting.
    + Shap - Untuk interpretasi model berbasis SHAP (Shapley Additive Explanations).
    + Joblib - Untuk menyimpan dan memuat model machine learning.
- Environtment
    + Jupyter Notebook - Untuk eksplorasi data interaktif dan dokumentasi langkah-langkah proyek.

## 4. Struktur Proyek
├── README.md # Penjelasan singkat terkait proyek yang dibuat.

├── Data

│ ├── UsedCarsSA_Unclean_EN.csv # Dataset

│

├── Model

│ ├── model_CatBoost.joblib # Model Joblib

│

├── Notebook

│ ├── Used_Cars_Analysis.ipynb # Jupyter Notebook dari Proyek yang dibuat

│

└── requirements.txt # Requirements yang dibutuhkan

## 5. Ringkasan Temuan
### 5.1 Insight Bisnis
- Usia mobil, tipe, dan ukuran mesin mobil merupakan faktor utama yang memengaruhi harga mobil bekas.
- Model CatBoost menunjukkan performa terbaik dibandingkan model dasar lainnya dalam hal akurasi prediksi harga dengan nilai MAPE 15.82%.


### 5.2 Rekomendasi Tindakan 

1. Integrasikan model ini sebagai alat estimasi harga otomatis di **Syarah.com** untuk mempermudah penentuan harga jual dan beli yang lebih akurat.
2. Gunakan model untuk validasi harga otomatis dan beri notifikasi jika harga menyimpang dari estimasi.
3. Perbarui model secara berkala dengan data terbaru untuk menjaga relevansi dan responsivitas terhadap tren pasar.
4. Tambahkan fitur baru seperti riwayat servis kendaraan dan kondisi kendaraan (misalnya: bekas kecelakaan atau kebanjiran) untuk meningkatkan akurasi model.

### 5.3 Limitasi Model

1. Model ini belum mempertimbangkan kondisi visual kendaraan, seperti kerusakan atau kecelakaan.
2. Penghapusan outlier ekstrem membatasi prediksi harga untuk mobil mewah, langka, atau edisi kolektor.
3. Model ini tidak memperhitungkan faktor eksternal seperti musim, promosi dealer, atau fluktuasi ekonomi makro.
4. Model dilatih dengan data historis, bukan data real-time, sehingga terbatas dalam memprediksi perubahan harga jangka pendek.

---

Tableu: [UsedCarAnalysis](https://public.tableau.com/app/profile/satrio.prabowo/viz/UsedCarAnalysis-SyarahDashboard/Dashboard13?publish=yes )

![ss Tableu1](https://github.com/PurwadhikaDev/BetaGroup_JC_DS_FT_BSD_26_FinalProject/blob/main/Gambar%20Tableu/WhatsApp%20Image%202025-07-16%20at%2022.48.44_ffd1e29d.jpg)
![ss Tableu2](https://github.com/PurwadhikaDev/BetaGroup_JC_DS_FT_BSD_26_FinalProject/blob/main/Gambar%20Tableu/WhatsApp%20Image%202025-07-16%20at%2022.48.58_cce7a8d6.jpg)
![ss Tableu3](https://github.com/PurwadhikaDev/BetaGroup_JC_DS_FT_BSD_26_FinalProject/blob/main/Gambar%20Tableu/WhatsApp%20Image%202025-07-16%20at%2022.49.49_23c7ce9f.jpg)

---
Streamlit: [UsedCarAnalysis](https://betagroupjcdsftbsd26finalprojectgit-rxh9ycuj7yqnycydcxzbav.streamlit.app/)
![ss Streamlit](https://github.com/PurwadhikaDev/BetaGroup_JC_DS_FT_BSD_26_FinalProject/blob/main/Gambar%20Streamlit/WhatsApp%20Image%202025-07-16%20at%2023.29.31_51d2bdff.jpg)
