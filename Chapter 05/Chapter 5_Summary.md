# Chapter 5 - Support Vector Machines (SVM)

## 1. Support Vector Machines (SVM)
**Support Vector Machines (SVM)** adalah algoritma yang digunakan untuk klasifikasi dan regresi. SVM berusaha menemukan **hyperplane** yang memisahkan data ke dalam kelas-kelas yang berbeda dengan margin yang sebesar-besarnya. Dalam kasus data yang tidak dapat dipisahkan secara linear, SVM menggunakan **kernel tricks** untuk memetakan data ke ruang dimensi yang lebih tinggi.

## 2. SVM untuk Klasifikasi Linier
SVM mencari **hyperplane optimal** yang memisahkan dua kelas data dengan margin terbesar. Data yang berada di sisi berbeda dari hyperplane akan diklasifikasikan ke dalam kelas yang berbeda. SVM bertujuan memaksimalkan margin di antara kelas-kelas tersebut untuk meningkatkan kemampuan generalisasi model.

## 3. Margin dan Support Vectors
**Margin** adalah jarak antara hyperplane dan data terdekat dari kedua kelas, yang disebut **support vectors**. Support vectors adalah data yang paling penting untuk membentuk hyperplane, karena hanya data ini yang menentukan posisi dan orientasi hyperplane.

## 4. SVM dengan Margin Lunak (Soft Margin)
Dalam kenyataannya, data sering kali tidak dapat dipisahkan dengan sempurna. Oleh karena itu, **soft margin SVM** diperkenalkan, yang memungkinkan beberapa kesalahan (misalnya, beberapa data terklasifikasi secara salah) selama pelatihan, asalkan margin tetap dijaga besar. Regularisasi dilakukan untuk mengontrol kesalahan dan memastikan model tidak terlalu fit pada data pelatihan (overfitting).

## 5. Kernel Tricks
**Kernel tricks** memungkinkan SVM untuk mengatasi masalah non-linearitas. Dengan kernel, data dapat dipetakan ke dalam ruang dimensi yang lebih tinggi, di mana data yang tidak dapat dipisahkan secara linear dalam ruang asli mungkin dapat dipisahkan secara linear. Kernel yang umum digunakan antara lain:
- **Linear Kernel**
- **Polynomial Kernel**
- **Radial Basis Function (RBF) Kernel**
- **Sigmoid Kernel**

## 6. SVM untuk Klasifikasi Non-Linier
Untuk masalah klasifikasi non-linear, kernel digunakan untuk mentransformasikan data ke ruang dimensi yang lebih tinggi, di mana pemisahan kelas menjadi lebih mudah. Misalnya, **RBF Kernel** memungkinkan SVM untuk menangani data yang sangat kompleks.

## 7. SVM untuk Regresi (SVR)
SVM juga dapat digunakan untuk regresi, yang disebut **Support Vector Regression (SVR)**. Dalam SVR, tujuan adalah menemukan garis atau hyperplane yang meminimalkan kesalahan pada prediksi data, tetapi dengan batasan pada seberapa besar kesalahan yang diperbolehkan (menggunakan margin lunak).

## 8. Kompleksitas Komputasi dan Pengaturan Hyperparameter
SVM dapat menjadi komputasi yang mahal, terutama dengan jumlah data yang sangat besar. Oleh karena itu, **pemilihan kernel** dan **parameter tuning** sangat penting. Beberapa parameter yang perlu diatur adalah:
- **C**: Parameter regularisasi yang mengontrol margin dan kesalahan pada data pelatihan.
- **Gamma**: Parameter yang mengontrol jangkauan pengaruh satu data training.

Pencarian grid atau **Randomized Search** dapat digunakan untuk menemukan kombinasi hyperparameter yang optimal.

## 9. SVM dalam Praktek
SVM sering digunakan dalam masalah klasifikasi biner dan juga dalam aplikasi seperti **pengenalan wajah**, **deteksi email spam**, dan **pengenalan pola**. Selain itu, SVM juga bekerja sangat baik pada dataset kecil hingga menengah dengan dimensi tinggi.

## 10. Kesimpulan
**Support Vector Machines (SVM)** adalah algoritma yang sangat kuat untuk klasifikasi dan regresi, yang berfokus pada pemisahan data dengan margin terbesar. Dengan penggunaan kernel tricks, SVM dapat menangani masalah non-linear dengan efektif. Meskipun SVM dapat sangat komputasi-intensif, pengaturan hyperparameter yang tepat dan pemilihan kernel yang sesuai sangat penting untuk kinerja yang optimal.
