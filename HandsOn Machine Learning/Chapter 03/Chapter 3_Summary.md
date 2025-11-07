# Chapter 3 - Classification

## 1. Pengenalan Klasifikasi
Klasifikasi adalah tugas di mana model machine learning mencoba memprediksi kelas atau kategori untuk data input. Contohnya, dalam **klasifikasi biner**, model harus memprediksi apakah sebuah email adalah spam atau bukan spam. Dalam **klasifikasi multi-kelas**, model memprediksi kategori dari beberapa kelas, seperti mengklasifikasikan gambar ke dalam kategori "anjing," "kucing," atau "kuda."

## 2. MNIST - Dataset Klasifikasi Tangan
Dataset **MNIST** (Modified National Institute of Standards and Technology) adalah salah satu dataset yang sering digunakan untuk masalah klasifikasi, khususnya pengenalan angka tulisan tangan. Dataset ini berisi gambar angka dari 0 hingga 9 yang digunakan untuk melatih model klasifikasi.

## 3. Melatih Klasifikator Biner
Melatih model untuk klasifikasi biner melibatkan memberikan data yang sudah diberi label (spam atau bukan spam) untuk mengajarkan model cara membedakan kelas-kelas tersebut. Salah satu metode yang digunakan untuk klasifikasi biner adalah **Logistic Regression**.

## 4. Mengukur Kinerja Klasifikasi
Kinerja model klasifikasi diukur dengan berbagai metrik, termasuk:
- **Akurasi**: Persentase prediksi yang benar dari total prediksi.
- **Precision dan Recall**: Digunakan untuk menilai model dalam konteks ketidakseimbangan kelas. **Precision** mengukur berapa banyak prediksi positif yang benar, sementara **Recall** mengukur berapa banyak data positif yang berhasil ditemukan oleh model.
- **F1-Score**: Merupakan rata-rata harmonis dari precision dan recall, digunakan ketika ada ketidakseimbangan kelas.
- **Confusion Matrix**: Matriks yang menunjukkan jumlah prediksi yang benar dan salah untuk setiap kelas, memudahkan analisis kesalahan.

## 5. Trade-off Precision/Recall
Terkadang, meningkatkan **precision** dapat mengurangi **recall**, dan sebaliknya. **Precision/Recall trade-off** terjadi ketika kita mengatur ambang batas keputusan untuk memutuskan apakah prediksi masuk dalam kategori positif atau negatif. Ini adalah masalah yang sering terjadi pada dataset dengan kelas yang tidak seimbang.

## 6. Kurva ROC dan AUC
**Kurva ROC** (Receiver Operating Characteristic) digunakan untuk menilai kinerja model klasifikasi, sementara **AUC** (Area Under the Curve) mengukur seberapa baik model membedakan antara kelas positif dan negatif. Semakin tinggi AUC, semakin baik model dalam membedakan kelas.

## 7. Klasifikasi Multi-Kelas
Klasifikasi multi-kelas melibatkan masalah di mana ada lebih dari dua kelas. Teknik untuk klasifikasi multi-kelas sering kali menggunakan pendekatan seperti **One-vs-All** atau **One-vs-One**, di mana satu model digunakan untuk setiap kelas atau pasangan kelas.

## 8. Analisis Kesalahan
Analisis kesalahan dilakukan untuk memahami mengapa model salah dalam memprediksi beberapa data. Dengan memeriksa jenis kesalahan yang dilakukan model, kita dapat memperbaiki atau meningkatkan model untuk mendapatkan hasil yang lebih baik.

## 9. Klasifikasi Multi-Label
**Klasifikasi multi-label** adalah tugas di mana setiap instance dapat memiliki lebih dari satu label. Misalnya, dalam klasifikasi berita, sebuah artikel mungkin bisa termasuk dalam kategori "politik" dan "ekonomi" secara bersamaan. Model multi-label akan menghasilkan lebih dari satu label untuk setiap instance.

## 10. Kesimpulan
Klasifikasi adalah salah satu tugas utama dalam machine learning yang digunakan untuk memprediksi kategori dari data. Menggunakan teknik dan metrik yang tepat sangat penting untuk melatih model yang efektif. Evaluasi model menggunakan metrik seperti **precision**, **recall**, **F1-score**, dan **AUC-ROC** sangat penting untuk memastikan kinerja model dalam berbagai skenario.
