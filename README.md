# 📊 Analisis Klasifikasi Nasabah

Notebook ini melakukan analisis dan pengelompokan data nasabah menggunakan teknik unsupervised learning. Fokus utama adalah pada pemrosesan data, reduksi dimensi, dan pengelompokan dengan algoritma K-Means.

## 🧰 Tools & Library
- **Pandas**, **NumPy**: manipulasi dan analisis data
- **Matplotlib**, **Seaborn**: visualisasi data
- **Scikit-learn**: encoding, normalisasi, PCA, dan KMeans
- **Feature-engine**: penanganan outlier menggunakan Winsorizer

## 📂 Dataset
Dataset terdiri dari fitur-fitur berikut:
- Usia
- Jenis kelamin
- Pendapatan
- Kategori kartu
- Status pernikahan
- Tingkat pendidikan

Langkah-langkah yang dilakukan:
1. **Eksplorasi Data Awal (EDA)**:
   - Cek dimensi dan informasi dataset
   - Visualisasi distribusi data numerikal dan kategorikal

2. **Penanganan Missing Value**:
   - Pengecekan dan pengisian data yang hilang

3. **Encoding Fitur Kategorikal**:
   - Menggunakan Label Encoding karena data tidak memiliki urutan yang jelas

4. **Handling Outlier**:
   - Menggunakan Winsorizer (metode IQR) untuk mereduksi pengaruh outlier

5. **Normalisasi Data**:
   - Standarisasi nilai agar memiliki skala yang seragam

6. **Reduksi Dimensi**:
   - Menggunakan Principal Component Analysis (PCA) untuk menyederhanakan data menjadi 2 dimensi utama

7. **Clustering**:
   - Menentukan jumlah cluster optimal dengan Elbow Method
   - Menerapkan KMeans clustering dengan 4 cluster
   - Evaluasi hasil clustering menggunakan Silhouette Coefficient

## 📈 Hasil
- Data berhasil direduksi menjadi 2 dimensi utama dengan PCA
- Jumlah cluster optimal adalah **4**
- Visualisasi hasil clustering menunjukkan pemisahan yang cukup baik antar kelompok

## 💡 Kesimpulan
Proses ini memungkinkan pengelompokan nasabah ke dalam beberapa segmen berdasarkan karakteristik demografis dan ekonomi. Hasil clustering dapat dimanfaatkan untuk strategi pemasaran, analisis risiko, atau personalisasi layanan.
