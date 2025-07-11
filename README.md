# Analisis dan Prediksi Harga Rumah di Ames, Iowa

Proyek ini bertujuan untuk membangun model machine learning yang dapat memprediksi harga jual rumah di Ames, Iowa, berdasarkan fitur-fitur properti. Dengan menggunakan dataset dari kompetisi Kaggle, dilakukan analisis data eksploratif, pembersihan data, dan pemodelan regresi. Model terbaik yang dihasilkan adalah Random Forest Regressor dengan nilai RMSE (Root Mean Squared Error) sebesar $29,480.

### 🎯 Masalah dan Tujuan
Perusahaan real estat seringkali kesulitan menentukan harga properti yang kompetitif dan akurat. Proyek ini bertujuan untuk:
1.  Mengidentifikasi faktor-faktor utama yang paling memengaruhi harga rumah.
2.  Membangun sebuah model otomatis untuk memberikan estimasi harga yang dapat diandalkan bagi agen dan klien.

### 💾 Sumber Data
Dataset yang digunakan berasal dari kompetisi Kaggle "House Prices: Advanced Regression Techniques". Anda dapat mengunduhnya [di sini](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).

### 🛠️ Teknologi yang Digunakan
* **Python 3.8**
* **Pandas & NumPy** untuk manipulasi data
* **Matplotlib & Seaborn** untuk visualisasi
* **Scikit-learn** untuk pemodelan dan evaluasi
* **Jupyter Notebook** sebagai lingkungan pengembangan

### 🚀 Alur Kerja Proyek
1.  **Pemuatan dan Pembersihan Data:** Menangani nilai yang hilang (*missing values*) dan memperbaiki tipe data.
2.  **Analisis Data Eksploratif (EDA):** Mencari pola dan wawasan melalui visualisasi, seperti distribusi harga, heatmap korelasi, dan boxplot.
3.  **Feature Engineering:** Memilih fitur-fitur yang paling relevan untuk model.
4.  **Pemodelan:** Melatih beberapa model regresi (Linear Regression, Random Forest).
5.  **Evaluasi Model:** Membandingkan performa model menggunakan metrik RMSE pada data uji.

6.  ### 📊 Hasil
Model Random Forest memberikan performa terbaik dibandingkan dengan Regresi Linear.

| Model                 | RMSE (USD)  |
| --------------------- | ----------- |
| Regresi Linear        | $35,294.78 |
| **Random Forest** | **$29,480.15** |

Fitur `OverallQual` (kualitas keseluruhan) dan `GrLivArea` (luas area tinggal) terbukti menjadi prediktor harga yang paling kuat.

![Heatmap Korelasi](visualizations/correlation_heatmap.png)
### 💻 Cara Menjalankan
1.  **Clone repository ini:**
    `git clone https://github.com/your-username/project-name.git`
2.  **Masuk ke direktori proyek:**
    `cd project-name`
3.  **Install semua library yang dibutuhkan:**
    `pip install -r requirements.txt`
4.  **Buka file notebook:**
    Buka folder `notebooks/` dan jalankan file `.ipynb` menggunakan Jupyter Notebook.
