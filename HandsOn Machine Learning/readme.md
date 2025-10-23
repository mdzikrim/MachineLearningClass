# Chatper 2 - End-to-End Proyek Machine Learning

## 1. Proyek Machine Learning End-to-End

Bab ini mengilustrasikan proyek ML yang melibatkan **prediksi harga rumah** dengan data yang mencakup berbagai tahapan, dari pengumpulan data hingga evaluasi model. Tujuan utama bab ini adalah untuk memberikan gambaran yang jelas tentang proses lengkap dalam membangun model ML di dunia nyata.

## 2. Pengumpulan dan Persiapan Data

- **Pengumpulan Data**: Data dikumpulkan melalui API atau dataset yang tersedia, misalnya dataset harga rumah yang akan digunakan untuk model regresi.
- **Pembersihan Data**: Langkah penting untuk memastikan kualitas data yang baik, mencakup penanganan nilai yang hilang, penghapusan data duplikat, serta pengecekan anomali dalam data.
- **Transformasi Data**: Data perlu ditransformasikan agar sesuai dengan algoritma ML yang dipilih. Misalnya, mengubah data kategori atau teks menjadi format numerik yang bisa diproses oleh model.

## 3. Membangun dan Melatih Model

Menggunakan **Scikit-Learn**, model regresi seperti **Linear Regression**, **Decision Trees**, dan **Random Forests** dibangun dan dilatih menggunakan data yang telah diproses. Setiap model diuji dengan data yang terpisah untuk mengevaluasi kinerjanya.

## 4. Evaluasi Model

Setelah model dilatih, **evaluasi model** dilakukan menggunakan metrik seperti **Mean Squared Error (MSE)** untuk regresi. Ini digunakan untuk mengukur seberapa akurat model dalam memprediksi data baru.

- **Cross-validation** juga diterapkan untuk memastikan bahwa model dapat menggeneralisasi dengan baik dan tidak hanya bekerja dengan baik pada data pelatihan.

## 5. Pemilihan Model Terbaik

Model terbaik dipilih berdasarkan performa yang telah dievaluasi menggunakan cross-validation dan metrik evaluasi lainnya. Beberapa model dicoba, dan model yang memberikan hasil terbaik dipilih untuk digunakan lebih lanjut dalam proyek.

## 6. Tuning Hyperparameter

Proses **tuning hyperparameter** dilakukan menggunakan teknik **Grid Search** atau **Random Search** untuk menemukan kombinasi parameter yang optimal untuk model, yang bertujuan untuk meningkatkan akurasi prediksi.

## 7. Pipeline dan Automasi

- **Pipeline** di Scikit-Learn digunakan untuk menyatukan berbagai langkah dalam transformasi data dan pelatihan model. Dengan pipeline, proses dapat dikelola dengan lebih efisien dan mudah diulang.
- Pipeline ini memungkinkan pengujian model secara sistematis, mengurangi kemungkinan kesalahan, dan memastikan model dapat digunakan dengan lebih mudah.

## 8. Pengujian Akhir dan Deployment

Setelah model selesai dioptimalkan, langkah terakhir adalah **deployment**, di mana model diterapkan untuk memprediksi data baru. Proses ini melibatkan pengujian model di dunia nyata dan memonitor performanya setelah deployment.

## 9. Menghindari Overfitting

Salah satu tantangan utama dalam **Machine Learning** adalah **overfitting**, di mana model terlalu cocok dengan data pelatihan dan tidak bisa digeneralisasi pada data baru. Beberapa teknik untuk menghindari overfitting antara lain:
- **Regularization**
- **Early stopping**
- **Cross-validation**
