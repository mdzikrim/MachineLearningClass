# Chapter 7 - Ensemble Learning and Random Forests=

## 1. Pengenalan Ensemble Learning
**Ensemble Learning** adalah teknik di mana beberapa model digunakan untuk membuat prediksi dan hasil prediksi mereka digabungkan untuk menghasilkan keputusan akhir yang lebih akurat. Teknik ini biasanya memberikan hasil yang lebih baik dibandingkan dengan model tunggal karena dapat mengurangi kesalahan yang dihasilkan oleh model individual.

Ada dua jenis utama ensemble learning:
- **Bagging (Bootstrap Aggregating)**: Menggunakan data pelatihan yang berbeda untuk melatih beberapa model dan menggabungkan hasilnya.
- **Boosting**: Melatih model secara berurutan, dengan model berikutnya fokus pada kesalahan yang dilakukan oleh model sebelumnya.

## 2. Voting Classifiers
**Voting classifiers** adalah metode ensemble yang menggunakan model yang berbeda untuk membuat prediksi dan menggabungkan hasilnya berdasarkan suara mayoritas. Ada dua jenis voting:
- **Hard Voting**: Setiap model memberikan satu suara, dan kelas yang memiliki suara terbanyak dipilih.
- **Soft Voting**: Setiap model memberikan probabilitas untuk setiap kelas, dan kelas dengan probabilitas tertinggi dipilih.

## 3. Bagging dan Pasting
**Bagging** (Bootstrap Aggregating) adalah teknik di mana banyak model dilatih secara paralel menggunakan subset acak dari data pelatihan. **Pasting** mirip dengan bagging, tetapi tanpa penggantian dalam pemilihan data. Bagging membantu mengurangi varians dan mencegah overfitting.

**Random Forests** adalah contoh utama dari metode bagging. Random Forests menggunakan banyak **decision trees** yang dilatih pada subset acak dari data dan fitur. Hasil prediksi dari setiap pohon digabungkan untuk menghasilkan keputusan akhir.

## 4. Random Forests
**Random Forests** adalah algoritma ensemble yang menggabungkan banyak **decision trees** untuk meningkatkan akurasi dan stabilitas. Setiap pohon dalam **Random Forest** dilatih pada subset acak dari data pelatihan dan subset acak dari fitur. Hal ini membuat Random Forests lebih robust terhadap overfitting dan lebih stabil dibandingkan dengan decision trees tunggal.

Beberapa keuntungan dari **Random Forests**:
- **Robust terhadap overfitting**: Dengan menggunakan banyak pohon, Random Forests lebih tahan terhadap overfitting.
- **Dapat menangani data yang hilang**: Random Forests dapat menangani data yang hilang dengan baik.
- **Evaluasi pentingnya fitur**: Random Forests dapat memberikan informasi tentang seberapa penting fitur dalam membuat prediksi.

## 5. Extra-Trees
**Extra-Trees** (Extremely Randomized Trees) adalah varian dari Random Forests yang lebih acak dalam memilih pembagian fitur. Extra-Trees menggunakan pembagian fitur yang lebih acak dan cepat, yang membuat algoritma ini lebih cepat dalam pelatihan, tetapi mungkin sedikit mengorbankan akurasi dibandingkan dengan Random Forests.

## 6. Feature Importance
**Random Forests** memiliki kemampuan untuk mengevaluasi **feature importance**—mengukur seberapa penting setiap fitur dalam membuat prediksi. Ini dapat digunakan untuk melakukan seleksi fitur dan mengurangi dimensi dataset tanpa kehilangan informasi penting.

## 7. Boosting
**Boosting** adalah metode ensemble yang melatih model secara berurutan, dengan model berikutnya memberikan bobot lebih pada kesalahan yang dilakukan oleh model sebelumnya. Beberapa algoritma boosting yang populer termasuk:
- **AdaBoost (Adaptive Boosting)**: Melatih model secara berurutan, memberi bobot lebih pada data yang salah diklasifikasikan oleh model sebelumnya.
- **Gradient Boosting**: Membangun model secara berurutan dengan mengoptimalkan fungsi kerugian menggunakan gradient descent.

## 8. Stacking
**Stacking** adalah metode ensemble yang menggabungkan hasil prediksi dari beberapa model menggunakan model lain untuk membuat prediksi akhir. Model-level pertama mengeluarkan prediksi yang digabungkan, dan model-level kedua (metamodel) mengambil hasil tersebut untuk membuat keputusan akhir. Stacking sering kali memberikan hasil yang lebih baik daripada teknik ensemble lainnya.

## 9. Kesimpulan
**Ensemble Learning** adalah pendekatan yang kuat untuk meningkatkan akurasi dan stabilitas model machine learning. Teknik seperti **bagging**, **boosting**, dan **stacking** menggabungkan kekuatan beberapa model untuk memberikan hasil yang lebih baik. **Random Forests** adalah contoh terkenal dari ensemble learning yang menggunakan banyak decision trees untuk meningkatkan ketahanan dan akurasi model, sementara **AdaBoost** dan **Gradient Boosting** menunjukkan kekuatan **boosting** dalam meningkatkan kinerja prediksi.
