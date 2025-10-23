# Chapter 1 - The Machine Learning Landscape

## 1. Apa Itu Machine Learning?

**Machine Learning (ML)** adalah ilmu (dan seni) untuk memprogram komputer agar dapat belajar dari data tanpa diprogram secara eksplisit. ML memungkinkan komputer untuk memperbaiki kinerjanya dalam suatu tugas tertentu melalui pengalaman yang diperoleh dari data.

Contoh sederhana dari **Machine Learning** adalah **filter spam** pada email. Filter ini belajar dari contoh email yang sudah diberi label (spam atau bukan spam), dan kemudian menggunakan informasi tersebut untuk memprediksi apakah email baru termasuk spam atau tidak.

## 2. Mengapa Menggunakan Machine Learning?

Dibandingkan dengan teknik pemrograman tradisional, **Machine Learning** menawarkan solusi untuk masalah yang sangat kompleks yang memerlukan pembaruan yang sering. Sebagai contoh, pada kasus filter spam, pemrograman tradisional mengharuskan pembuatan banyak aturan secara manual untuk mengenali spam. Hal ini menjadi sulit untuk dipelihara dan diupdate. Sebaliknya, filter spam berbasis ML dapat menyesuaikan diri dengan pola baru dalam spam tanpa perlu intervensi programmer.

**Machine Learning** juga sangat berguna untuk masalah yang lebih kompleks, seperti **pengenalan suara** atau **pengolahan bahasa alami** (NLP), yang mana pendekatan tradisional tidak dapat menangani masalah tersebut secara efektif.

## 3. Contoh Aplikasi Machine Learning

Berikut adalah beberapa contoh aplikasi ML dalam kehidupan sehari-hari:

- **Klasifikasi gambar** pada jalur produksi untuk mengidentifikasi produk.
- **Deteksi tumor** dalam scan otak (menggunakan teknik segmentasi semantik).
- **Klasifikasi artikel berita otomatis** (aplikasi dalam NLP).
- **Mendeteksi penipuan kartu kredit** (deteksi anomali).
- **Memprediksi pendapatan perusahaan** tahun depan (regresi).
- **Membangun chatbot atau asisten pribadi** (menggunakan NLP dan pengolahan suara).

## 4. Tipe-Tipe Sistem Machine Learning

Machine Learning dapat diklasifikasikan berdasarkan beberapa kriteria berikut:

- **Supervised Learning**: Sistem belajar dari data berlabel, di mana model dilatih dengan contoh yang memiliki label yang sudah diketahui (misalnya, klasifikasi spam dan prediksi harga mobil).
- **Unsupervised Learning**: Sistem belajar tanpa label, mencari pola atau struktur dalam data (misalnya, klastering untuk segmentasi pelanggan).
- **Semi-supervised Learning**: Gabungan dari kedua pendekatan sebelumnya, di mana sebagian besar data tidak memiliki label.
- **Reinforcement Learning**: Sistem belajar dengan cara berinteraksi dengan lingkungan dan menerima umpan balik berupa penghargaan atau hukuman berdasarkan tindakannya (contoh: permainan Go oleh AlphaGo).

## 5. Batch vs. Online Learning

- **Batch Learning**: Sistem dilatih menggunakan seluruh data yang tersedia sekaligus. Proses ini memerlukan waktu dan sumber daya yang besar, sehingga sering dilakukan secara offline. Jika ingin menambahkan data baru, sistem harus dilatih ulang dari awal.
- **Online Learning**: Sistem belajar secara bertahap dari data yang datang secara terus-menerus. Ini cocok untuk situasi di mana data berubah seiring waktu dan memerlukan model yang bisa beradaptasi dengan cepat.

## 6. Tantangan Utama dalam Machine Learning

Beberapa tantangan utama dalam **Machine Learning** antara lain:

- **Data tidak cukup**: Jika data yang tersedia terlalu sedikit atau kurang representatif, model tidak dapat dilatih dengan baik.
- **Data yang tidak representatif**: Data yang tidak mencerminkan keadaan sesungguhnya atau data yang bias dapat menyebabkan model yang buruk.
- **Overfitting dan Underfitting**: Overfitting terjadi ketika model terlalu cocok dengan data pelatihan dan tidak dapat digeneralisasi pada data baru, sementara underfitting terjadi ketika model terlalu sederhana untuk menangkap pola dalam data.

## 7. Proses Kerja Proyek Machine Learning

Proyek ML tipikal melibatkan beberapa langkah berikut:

- **Pengumpulan data**: Mengambil data yang relevan untuk masalah yang akan diselesaikan.
- **Persiapan data**: Membersihkan dan mengubah data ke format yang cocok untuk pelatihan.
- **Pemilihan model**: Memilih model yang paling cocok untuk masalah yang dihadapi.
- **Pelatihan model**: Melatih model dengan data pelatihan.
- **Evaluasi dan penyesuaian model**: Menggunakan data uji untuk mengevaluasi kinerja model dan menyesuaikan hyperparameter atau memilih model yang lebih baik.

## 8. Mengevaluasi dan Menyempurnakan Sistem Machine Learning

Proses evaluasi dan penyempurnaan model sangat penting untuk memastikan model ML bekerja dengan baik. Teknik seperti **validasi silang** dan **tuning hyperparameter** diperlukan untuk memperoleh model yang optimal dan menghindari masalah **overfitting**.
