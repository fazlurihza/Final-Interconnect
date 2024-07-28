# Laporan Tugas

**Deskripsi Proyek**

Proyek ini bertujuan untuk memprediksi churn pelanggan bagi perusahaan telekomunikasi Interconnect. Jika diketahui bahwa seorang pelanggan berencana untuk meninggalkan layanan, maka mereka akan ditawarkan kode promosi dan opsi paket khusus. Kami menggunakan data pelanggan, informasi kontrak, dan layanan untuk membangun model prediksi. Deskripsi Data

Data terdiri dari empat file yang berisi informasi mengenai kontrak, data pribadi, layanan internet, dan layanan telepon. Semua file tersebut digabungkan menggunakan kolom customerID.

Data Initialization:

Mengimpor data dari empat file CSV: contract.csv, personal.csv, internet.csv, dan phone.csv.
Data Preparation and Cleaning:

Menggabungkan data dari keempat file berdasarkan customerID.
Menangani nilai yang hilang dan mengubah tipe data yang diperlukan.
Membuat variabel target Churn berdasarkan kolom EndDate.
Preliminary EDA:

Analisis distribusi biaya bulanan (MonthlyCharges) antara pelanggan yang churn dan yang tidak churn.
Visualisasi data menggunakan histogram dan boxplot untuk memahami distribusi dan outlier.
Masalah

Data yang hilang pada beberapa kolom.
Variabel dengan tipe data yang tidak sesuai.
Menentukan variabel yang signifikan untuk model prediksi.

**Tujuan**

Memprediksi churn pelanggan dengan akurasi yang tinggi.
Mengidentifikasi faktor-faktor yang mempengaruhi churn pelanggan.

**Metodologi**

Variance Testing, Statistical Testing

Melakukan uji statistik seperti uji t untuk menentukan perbedaan signifikan antara kelompok churn dan non-churn.
Analisis korelasi untuk menemukan hubungan antara variabel independen dan variabel target.
Definisi Metodologi

Supervised learning dengan menggunakan beberapa algoritma: Logistic Regression, Random Forest, dan Gradient Boosting.
Evaluasi model menggunakan metrik AUC-ROC dan akurasi.
Pemilihan model terbaik berdasarkan performa metrik.

**Literatur Review**

Studi sebelumnya menunjukkan bahwa model prediksi churn yang efektif dapat membantu perusahaan dalam mengembangkan strategi retensi pelanggan yang lebih baik.
Algoritma machine learning seperti Logistic Regression dan Random Forest sering digunakan dalam prediksi churn.
Hasil

**EDA**

Distribusi biaya bulanan (MonthlyCharges) menunjukkan bahwa pelanggan yang churn cenderung memiliki biaya bulanan yang lebih tinggi dibandingkan dengan pelanggan yang tidak churn.
Visualisasi distribusi dan outlier menggunakan boxplot dan histogram.

**Analisis Statistik**

Uji t menunjukkan perbedaan signifikan dalam biaya bulanan antara kelompok churn dan non-churn.
Analisis korelasi menunjukkan beberapa variabel yang memiliki korelasi signifikan dengan variabel target.
Pemodelan

Melatih model menggunakan Logistic Regression, Random Forest, dan Gradient Boosting.
Evaluasi model menggunakan AUC-ROC dan akurasi.

**Hasil Evaluasi Model:**

Logistic Regression - AUC-ROC: 0.8359, Accuracy: 0.7941
Random Forest - AUC-ROC: 0.8123, Accuracy: 0.7780
Gradient Boosting - AUC-ROC: 0.8406, Accuracy: 0.7951

**Evaluasi Model**

Model Gradient Boosting menunjukkan performa terbaik dengan AUC-ROC sebesar 0.8406 dan akurasi 0.7951.
Evaluasi model menunjukkan bahwa model ini dapat membedakan antara pelanggan yang churn dan yang tidak dengan baik.

**Diskusi**

Analisis Langkah yang Dilakukan dan Tidak Dilakukan

Langkah yang Dilakukan:

Persiapan dan pembersihan data
Analisis data eksploratif (EDA)
Uji statistik dan analisis korelasi
Pelatihan dan evaluasi model
Pemilihan model terbaik
Langkah yang Tidak Dilakukan:

Tuning hyperparameter lebih lanjut dikarenakan keterbatasan waktu
Penggunaan validasi silang karena data yang terbatas

**Kesulitan yang Dihadapi**

Menangani nilai yang hilang dan tipe data yang tidak sesuai.
Solusi: Menggunakan imputasi nilai dan konversi tipe data yang sesuai.
Memilih fitur yang paling relevan untuk model prediksi.
Solusi: Menggunakan analisis korelasi dan uji statistik.

**Langkah Kunci untuk Menyelesaikan Tugas**

Pembersihan dan persiapan data yang menyeluruh.
Analisis data eksploratif untuk memahami distribusi dan hubungan antar variabel.
Evaluasi model yang komprehensif menggunakan berbagai metrik.

**Model Akhir dan Skor Kualitas**

Model akhir: Gradient Boosting
Skor kualitas: AUC-ROC 0.8406, Akurasi 0.7951

**Kesimpulan**

Proyek ini berhasil mencapai tujuan utama yaitu memprediksi churn pelanggan dengan akurasi dan AUC-ROC yang memadai. Model Gradient Boosting terbukti menjadi pilihan terbaik dalam memprediksi churn pelanggan Interconnect. Dengan rekomendasi yang diberikan, perusahaan dapat meningkatkan model lebih lanjut dan mengembangkan strategi retensi pelanggan yang lebih efektif, yang pada akhirnya dapat mengurangi churn dan meningkatkan kepuasan pelanggan. Rekomendasi

Melakukan tuning hyperparameter lebih lanjut untuk meningkatkan performa model.
Menambahkan lebih banyak fitur yang relevan yang dapat membantu dalam memprediksi churn.
Melakukan validasi silang untuk memastikan model tidak overfitting.
Melakukan penelitian lebih lanjut untuk memahami alasan pelanggan melakukan churn dan mengembangkan strategi retensi yang lebih efektif.
