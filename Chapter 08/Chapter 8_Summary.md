# Chapter 8 - Dimensionality Reduction

## 1. Pengenalan Dimensionality Reduction
**Dimensionality Reduction** adalah proses mengurangi jumlah fitur dalam dataset tanpa mengorbankan terlalu banyak informasi. Ini dapat membantu meningkatkan kinerja model machine learning, mempercepat pelatihan, dan mengurangi risiko overfitting.

Beberapa alasan untuk menggunakan dimensionality reduction adalah:
- **Mengurangi kompleksitas model**: Dengan lebih sedikit fitur, model menjadi lebih sederhana dan lebih mudah dipahami.
- **Meningkatkan efisiensi komputasi**: Dataset dengan dimensi yang lebih rendah membutuhkan lebih sedikit sumber daya untuk diproses.
- **Mengurangi overfitting**: Mengurangi dimensi data dapat mengurangi noise dan membantu model generalisasi lebih baik.

## 2. Curse of Dimensionality
**Curse of Dimensionality** mengacu pada fenomena di mana data dengan dimensi yang sangat tinggi (banyak fitur) dapat menyebabkan masalah dalam analisis dan model machine learning. Semakin tinggi dimensi data, semakin sulit untuk menemukan pola yang berguna, karena data menjadi tersebar di ruang fitur yang sangat besar.

## 3. Proyeksi dan Manifold Learning
Dimensionality reduction dapat dilakukan dengan **proyeksi** data ke ruang dengan dimensi yang lebih rendah. Beberapa pendekatan untuk proyeksi termasuk **Principal Component Analysis (PCA)**, **Linear Discriminant Analysis (LDA)**, dan **t-SNE**. 

Selain itu, teknik **Manifold Learning** berusaha untuk menangkap struktur data yang lebih kompleks yang tidak dapat dijelaskan hanya dengan proyeksi linier. Teknik ini termasuk **Isomap**, **LLE (Locally Linear Embedding)**, dan **t-SNE (t-Distributed Stochastic Neighbor Embedding)**.

## 4. Principal Component Analysis (PCA)
**PCA** adalah teknik dimensionality reduction yang paling banyak digunakan. PCA mengidentifikasi komponen utama (principal components) yang menjelaskan variansi terbesar dalam data, dan memproyeksikan data ke dalam ruang fitur yang lebih rendah berdasarkan komponen-komponen ini.

Langkah-langkah dalam PCA:
- Menghitung **covariance matrix** untuk mengidentifikasi hubungan antara fitur.
- Menghitung **eigenvector** dan **eigenvalue** untuk menemukan komponen utama.
- Memilih komponen utama yang menjelaskan sebagian besar variansi dan memproyeksikan data ke ruang dimensi yang lebih rendah.

PCA sangat efektif untuk mengurangi dimensi data, terutama ketika fitur-fitur dalam data saling berkorelasi.

## 5. Kernel PCA
**Kernel PCA** adalah varian dari PCA yang menggunakan **kernel tricks** untuk melakukan dimensionality reduction pada data non-linear. Teknik ini memungkinkan PCA untuk menangani data yang tidak dapat dipisahkan secara linier dengan memetakan data ke dalam ruang dimensi yang lebih tinggi.

## 6. LLE (Locally Linear Embedding)
**LLE** adalah teknik manifold learning yang mencoba untuk mempertahankan struktur lokal data dengan mengurangi dimensi. LLE berfokus pada hubungan antar data yang berdekatan dan menganggap bahwa data berada pada manifold yang lebih rendah. LLE efektif untuk menangkap pola yang ada dalam data dengan dimensi tinggi.

## 7. t-SNE (t-Distributed Stochastic Neighbor Embedding)
**t-SNE** adalah teknik dimensionality reduction yang sangat efektif untuk visualisasi data. t-SNE mengubah data ke dalam dimensi dua atau tiga sehingga pola dalam data dapat divisualisasikan dalam grafik. t-SNE mempertahankan hubungan jarak antar data poin dalam ruang dimensi yang lebih rendah, yang membuatnya sangat berguna untuk eksplorasi visual data.

## 8. Penggunaan Dimensionality Reduction dalam Machine Learning
Dimensionality reduction sangat berguna dalam machine learning, terutama ketika data memiliki banyak fitur yang tidak semuanya relevan atau berguna. Beberapa keuntungan dari menggunakan dimensionality reduction termasuk:
- **Peningkatan kinerja algoritma**: Dengan mengurangi jumlah fitur, algoritma machine learning dapat bekerja lebih cepat dan lebih efisien.
- **Pengurangan overfitting**: Dengan mengurangi dimensi, model dapat lebih baik dalam generalisasi dan menghindari overfitting pada data pelatihan.
- **Visualisasi data**: Teknik seperti PCA dan t-SNE memungkinkan visualisasi data yang lebih mudah dipahami, terutama untuk dataset yang sangat besar.

## 9. Kesimpulan
**Dimensionality Reduction** adalah teknik penting dalam machine learning yang dapat membantu mengurangi jumlah fitur dalam dataset dan meningkatkan efisiensi serta kinerja model. Teknik seperti **PCA**, **Kernel PCA**, **LLE**, dan **t-SNE** dapat digunakan untuk berbagai tujuan, mulai dari mempercepat pelatihan model hingga memvisualisasikan data yang kompleks. Pemilihan teknik yang tepat bergantung pada sifat data dan tujuan analisis.
