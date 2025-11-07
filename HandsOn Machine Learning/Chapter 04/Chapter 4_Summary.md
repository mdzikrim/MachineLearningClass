# Chapter 4: Training Models - Rangkuman

Chapter ini membahas teknik-teknik yang digunakan untuk melatih model machine learning secara efektif. Berikut adalah poin-poin penting yang dibahas:

## 1. Training Model
Pelatihan model adalah inti dari proyek machine learning yang melibatkan pembuatan dan optimasi model untuk menghasilkan prediksi berdasarkan data. Berbagai algoritma dapat digunakan, dari regresi linier hingga jaringan saraf dalam.

## 2. Fungsi Biaya (Cost Function) dan Optimasi
Model machine learning berusaha mengurangi kesalahan antara prediksi yang dihasilkan dan nilai yang benar dengan menggunakan **cost function**. Teknik **Gradient Descent** digunakan untuk mengoptimalkan model dengan cara mengubah parameter secara bertahap untuk mencapai nilai optimal.

## 3. Regularisasi
Regularisasi adalah teknik untuk mencegah **overfitting** pada model, di mana model terlalu menyesuaikan data pelatihan dan tidak dapat menggeneralisasi dengan baik pada data baru. Beberapa teknik yang digunakan:
- **L1 Regularization (Lasso)**: Membantu seleksi fitur dengan mendorong beberapa parameter menjadi nol.
- **L2 Regularization (Ridge)**: Menambahkan penalti untuk parameter besar, menjaga model tetap sederhana.
- **Dropout**: Digunakan dalam jaringan saraf untuk mencegah overfitting dengan mengabaikan beberapa neuron secara acak.

## 4. Hyperparameter Tuning
**Hyperparameter tuning** adalah proses pencarian nilai terbaik untuk parameter yang tidak dipelajari oleh model namun mempengaruhi pelatihan model. Teknik seperti **Grid Search** dan **Randomized Search** digunakan untuk menemukan kombinasi terbaik dari hyperparameter.

## 5. Regresi Lanjut
Teknik **Ridge Regression** dan **Lasso Regression** digunakan untuk mengatasi masalah seperti multikolinearitas dan overfitting dengan menambahkan penalti pada parameter model.

## 6. Support Vector Machines (SVM)
**Support Vector Machines (SVM)** digunakan untuk klasifikasi dan regresi. SVM bekerja dengan mencari hyperplane terbaik untuk memisahkan kelas dalam data. Untuk masalah non-linear, **kernel tricks** digunakan untuk meningkatkan kemampuan SVM dalam menemukan solusi yang lebih kompleks.

## 7. Evaluasi Model dan Kinerja
Evaluasi model dilakukan dengan menggunakan data uji untuk memastikan model dapat menggeneralisasi dengan baik. Teknik evaluasi seperti **Cross-validation** dan **Confusion Matrix** digunakan untuk mengukur kinerja model.

## 8. Mengatasi Overfitting dan Underfitting
**Overfitting** terjadi saat model terlalu kompleks, sedangkan **Underfitting** terjadi ketika model terlalu sederhana. Menyeimbangkan bias dan varians model sangat penting untuk memastikan performa yang baik pada data baru.

## 9. Optimasi Model
Optimasi model dilakukan dengan memilih model yang tepat, menyesuaikan hyperparameter, dan meningkatkan efisiensi agar model dapat menangani data lebih baik. **Cross-validation** digunakan untuk memastikan model dapat bekerja dengan baik pada data yang berbeda.

## 10. Kesimpulan
Setelah model dilatih dan dioptimalkan, penting untuk terus memantau kinerjanya dan melakukan evaluasi berkelanjutan untuk memastikan model tetap efektif pada data baru yang masuk.
