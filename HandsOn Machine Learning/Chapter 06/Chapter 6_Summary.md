# Chapter 6 - Decision Trees

## 1. Pengenalan Decision Trees
**Decision Trees** adalah model yang menyusun data dalam bentuk struktur pohon, di mana setiap cabang mewakili keputusan berdasarkan fitur tertentu dan setiap daun mewakili hasil prediksi (kelas atau nilai regresi). Decision Tree dapat digunakan untuk **klasifikasi** dan **regresi**, dengan model yang mudah dipahami dan diterapkan.

## 2. Membangun Decision Tree
Proses pembangunan Decision Tree dimulai dengan memilih fitur terbaik untuk membagi data pada setiap langkah (node). Kriteria pemilihan fitur yang umum digunakan adalah:
- **Gini Impurity**: Digunakan untuk klasifikasi biner, mengukur ketidakmurnian setiap node. Node yang memiliki Gini Impurity rendah lebih baik dalam membagi data ke dalam kelas yang benar.
- **Entropy dan Information Gain**: Digunakan untuk mengukur ketidakpastian dalam dataset. **Information Gain** mengukur pengurangan ketidakpastian (entropy) setelah melakukan pembagian data berdasarkan fitur tertentu.
- **Mean Squared Error (MSE)**: Digunakan untuk regresi, untuk mengukur perbedaan antara nilai yang diprediksi dan nilai aktual.

## 3. Algoritma CART (Classification and Regression Trees)
**CART** adalah algoritma yang sering digunakan untuk membangun Decision Trees. Pada CART, setiap percabangan pohon dilakukan untuk meminimalkan impurity atau error di node, dan pada akhirnya menghasilkan pohon biner.

## 4. Pruning pada Decision Tree
**Pruning** adalah teknik untuk mengurangi ukuran pohon dengan menghapus cabang-cabang yang tidak diperlukan. Tujuan utama pruning adalah untuk mencegah **overfitting**, yang dapat terjadi ketika pohon menjadi terlalu kompleks dan menyesuaikan terlalu banyak pada data pelatihan. Ada dua jenis pruning:
- **Pre-pruning**: Menghentikan pembagian lebih lanjut pada node tertentu jika pembagiannya tidak memberikan keuntungan yang signifikan.
- **Post-pruning**: Membangun pohon sepenuhnya dan kemudian memotong cabang yang tidak memberikan kontribusi penting untuk prediksi.

## 5. Keuntungan dan Kelemahan Decision Trees
### Keuntungan:
- Mudah dipahami dan diinterpretasikan, bahkan oleh non-expert.
- Dapat menangani data numerik dan kategorikal.
- Tidak memerlukan normalisasi atau scaling fitur.
  
### Kelemahan:
- Rentan terhadap **overfitting**, terutama ketika pohon terlalu dalam.
- Tidak stabil terhadap perubahan kecil pada data pelatihan, yang bisa mengubah struktur pohon secara signifikan.

## 6. Hyperparameter pada Decision Trees
Beberapa hyperparameter yang perlu diatur untuk Decision Tree antara lain:
- **Max Depth**: Kedalaman maksimal pohon, yang membatasi berapa banyak pembagian yang dapat dilakukan.
- **Min Samples Split**: Jumlah minimum sampel yang diperlukan untuk membagi sebuah node.
- **Min Samples Leaf**: Jumlah minimum sampel yang diperlukan di sebuah daun.
- **Max Features**: Jumlah maksimal fitur yang dipertimbangkan untuk setiap split.

Pengaturan yang tepat dari hyperparameter ini sangat penting untuk mencegah overfitting dan memastikan model bekerja dengan baik pada data yang belum terlihat.

## 7. Menggunakan Decision Trees dalam Praktek
Decision Trees dapat diterapkan dalam berbagai kasus seperti **analisis risiko**, **deteksi penipuan**, dan **pengenalan pola**. Model ini juga menjadi dasar bagi algoritma yang lebih kompleks, seperti **Random Forest** dan **Gradient Boosting**, yang menggabungkan banyak pohon untuk meningkatkan akurasi dan stabilitas.

## 8. Visualisasi Decision Trees
Salah satu kelebihan utama dari Decision Trees adalah kemampuannya untuk divisualisasikan, sehingga proses pengambilan keputusan dapat dipahami dengan jelas. Visualisasi ini sangat membantu dalam menjelaskan bagaimana model membuat prediksi berdasarkan fitur-fitur yang diberikan.

## 9. Kesimpulan
**Decision Trees** adalah algoritma yang kuat dan mudah dipahami untuk masalah klasifikasi dan regresi. Meskipun mereka memiliki kelemahan dalam hal overfitting dan stabilitas, teknik seperti **pruning** dan pengaturan hyperparameter dapat membantu mengatasi masalah tersebut. Dengan penggunaan yang tepat, Decision Trees dapat memberikan hasil yang sangat baik dan digunakan sebagai dasar untuk model yang lebih kompleks seperti Random Forest dan Gradient Boosting.
