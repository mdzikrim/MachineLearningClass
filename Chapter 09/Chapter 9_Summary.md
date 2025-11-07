# Chapter 9 - Unsupervised Learning Techniques

## 1. Pengenalan Unsupervised Learning
**Unsupervised Learning** adalah teknik di mana model belajar dari data yang tidak memiliki label atau kategori. Tujuannya adalah untuk menemukan pola atau struktur dalam data tanpa arahan eksplisit tentang hasil yang diinginkan. Teknik unsupervised learning termasuk **clustering**, **anomaly detection**, **dimensionality reduction**, dan **association rule learning**.

## 2. Clustering
**Clustering** adalah tugas unsupervised learning di mana data dikelompokkan ke dalam cluster berdasarkan kemiripan antar data. Clustering sangat berguna untuk eksplorasi data dan segmentasi.

### Jenis-Jenis Algoritma Clustering:
- **K-Means Clustering**: Algoritma yang membagi data ke dalam sejumlah cluster yang telah ditentukan sebelumnya dengan meminimalkan jarak antara data dan pusat cluster. K-Means mudah diterapkan dan efektif pada data yang relatif terpisah.
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**: Algoritma clustering yang mengelompokkan titik data berdasarkan kepadatan titik-titik tersebut. DBSCAN sangat berguna untuk data dengan bentuk cluster yang tidak teratur dan dapat mengidentifikasi titik data sebagai **noise** jika tidak cukup padat.
- **Hierarchical Clustering**: Algoritma yang membangun pohon cluster (dendrogram) dengan menggabungkan cluster secara hierarkis. Ini dapat digunakan untuk menentukan jumlah cluster secara otomatis dan melihat hubungan antar cluster pada berbagai tingkat hierarki.

## 3. Anomaly Detection
**Anomaly detection** adalah teknik untuk menemukan data yang menyimpang dari pola normal. Teknik ini sering digunakan dalam deteksi penipuan, pemeliharaan prediktif, dan identifikasi kegagalan sistem.

### Algoritma untuk Anomaly Detection:
- **One-Class SVM**: Algoritma yang memisahkan data normal dari data anomali dengan membangun sebuah batas yang memisahkan data dalam ruang fitur.
- **Isolation Forest**: Algoritma yang membangun pohon keputusan untuk mengisolasi data yang lebih jarang, sehingga titik yang lebih jarang (anomali) lebih cepat terisolasi dibandingkan titik yang lebih umum.

## 4. Dimensionality Reduction
**Dimensionality Reduction** adalah teknik untuk mengurangi jumlah fitur dalam dataset tanpa mengurangi informasi yang terlalu banyak. Teknik ini berguna untuk mempercepat pelatihan model dan visualisasi data.

### Teknik Dimensionality Reduction:
- **PCA (Principal Component Analysis)**: Mengidentifikasi komponen utama yang menjelaskan variansi terbesar dalam data dan memproyeksikan data ke ruang fitur yang lebih rendah.
- **t-SNE (t-Distributed Stochastic Neighbor Embedding)**: Digunakan untuk visualisasi data dengan memproyeksikan data berdimensi tinggi ke ruang dua atau tiga dimensi untuk melihat pola atau kelompok dalam data.

## 5. Association Rule Learning
**Association rule learning** adalah teknik yang digunakan untuk menemukan hubungan atau pola yang sering terjadi dalam dataset. Teknik ini sering digunakan dalam analisis pasar untuk menemukan asosiasi antar produk yang sering dibeli bersama.

### Algoritma untuk Association Rule Learning:
- **Apriori Algorithm**: Algoritma yang digunakan untuk menemukan asosiasi antar item dalam dataset, sering diterapkan dalam analisis transaksi.
- **Eclat Algorithm**: Algoritma yang lebih efisien daripada Apriori untuk menemukan itemset yang sering terjadi, dengan menggunakan teknik **depth-first search**.

## 6. Penggunaan Unsupervised Learning dalam Praktek
Unsupervised learning memiliki banyak aplikasi praktis, termasuk:
- **Segmentasi pasar**: Menggunakan clustering untuk mengelompokkan pelanggan berdasarkan perilaku atau preferensi mereka.
- **Pengenalan pola**: Menggunakan anomaly detection untuk mendeteksi aktivitas yang tidak biasa dalam data seperti transaksi yang mencurigakan.
- **Reduksi dimensi**: Menggunakan PCA untuk mengurangi jumlah fitur dalam dataset besar dan membuatnya lebih mudah untuk dianalisis dan divisualisasikan.
- **Rekomendasi produk**: Menggunakan association rule learning untuk merekomendasikan produk yang sering dibeli bersama oleh pelanggan.

## 7. Kesimpulan
**Unsupervised learning** memberikan kemampuan untuk menemukan pola atau struktur dalam data tanpa label. Teknik seperti **clustering**, **anomaly detection**, **dimensionality reduction**, dan **association rule learning** memungkinkan penemuan wawasan yang mendalam dalam berbagai domain. Dengan aplikasi yang luas, unsupervised learning menjadi alat yang sangat berharga dalam analisis data besar dan eksplorasi data.
