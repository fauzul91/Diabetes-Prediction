# Prediksi Diabetes

## Deskripsi Proyek
Repositori ini berisi proyek prediksi diabetes menggunakan dataset yang telah diproses melalui berbagai langkah, mulai dari pembersihan data hingga evaluasi model machine learning. Model utama yang digunakan adalah K-Nearest Neighbors (KNN), dengan evaluasi kinerja yang mencakup metrik seperti accuracy, precision, recall, dan F1 score. Proyek ini juga membandingkan kinerja model sebelum dan sesudah penanganan outlier, serta menerapkan metode SMOTE untuk mengatasi ketidakseimbangan data.

## Langkah-Langkah Proyek
### 1. Pembersihan Data (Data Cleaning)
- **Cek Missing Values:**
  - Dataset diperiksa untuk nilai yang hilang (missing values).
- **Penanganan Duplikasi Data:**
  - Data duplikat diidentifikasi dan dihapus untuk memastikan keakuratan dataset.

### 2. Preprocessing Data
- **Penyesuaian Kolom Gender:**
  - Melakukan transformasi data pada Kolom gender dan dikonversi menjadi nilai numerik untuk kompatibilitas dengan model machine learning.
- **Penyesuaian Kolom Class:**
  - Kolom target (class) dikategorikan ke dalam nilai yang sesuai untuk representasi binary yaitu 0 dan 1.
- **Identifikasi Outlier:**
  - Outlier dalam dataset diidentifikasi menggunakan metode statistik yaitu IQR.
  - Dataset disimpan dalam dua versi: sebelum dan sesudah penghapusan outlier.

### 3. Penanganan Ketidakseimbangan Data
- **Oversampling dengan SMOTE:**
  - Synthetic Minority Over-sampling Technique (SMOTE) diterapkan pada kolom class untuk menangani ketidakseimbangan data.

### 4. Pembuatan Model
- **Train-Test Split:**
  - Dataset dibagi menjadi data latih dan data uji dengan proporsi 80:20.
- **Membangun Model KNN:**
  - Model K-Nearest Neighbors dibangun dengan parameter default dan jumlah tetangga (n) = 5.

### 5. Evaluasi Model
- **Confusion Matrix:**
  - Confusion matrix digunakan untuk mengevaluasi performa model.
- **Metrik Evaluasi:**
  - **Accuracy:** Mengukur persentase prediksi yang benar.
  - **Precision:** Mengukur proporsi prediksi positif yang benar.
  - **Recall:** Mengukur kemampuan model untuk mendeteksi kelas positif.
  - **F1 Score:** Harmonic mean antara precision dan recall.

### 6. Perbandingan Model
- Model dibandingkan berdasarkan dataset sebelum dan sesudah penghapusan outlier untuk mengevaluasi pengaruh outlier terhadap performa model.

## Cara Menjalankan Proyek
1. Clone repositori:
   ```bash
   git clone https://github.com/fauzul91/Diabetes-Prediction.git
   ```

## Dependencies
- Python >= 3.8
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).

