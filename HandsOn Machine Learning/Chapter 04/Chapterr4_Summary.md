# 📘 Chapter 4 – Training Models (Exercise Answers)

---

## 1. Which Linear Regression training algorithm can you use if you have a training set with millions of features?
Menggunakan **Stochastic Gradient Descent (SGD)** karena efisien untuk dataset sangat besar dan bersifat online learning.

---

## 2. Suppose the features in your training set have very different scales. Which algorithms might suffer from this, and how? What can you do about it?
Algoritma seperti **Gradient Descent** sangat sensitif terhadap skala fitur karena gradien menjadi miring atau tidak stabil. Solusinya adalah melakukan **feature scaling** (misal: StandardScaler).

---

## 3. Can Gradient Descent get stuck in a local minimum when training a Logistic Regression model?
Pada **Logistic Regression** dan **Linear Regression**, fungsi cost-nya **convex**, jadi tidak memiliki local minimum, hanya satu global minimum. Gradient Descent tidak akan terjebak.

---

## 4. Do all Gradient Descent algorithms lead to the same model, provided you let them run long enough?
Ya, **dengan syarat learning rate cukup kecil dan dijalankan cukup lama**, semua variasi Gradient Descent akan menuju minimum yang sama (karena loss convex).

---

## 5. Suppose you use Batch Gradient Descent and you plot the validation error at every epoch. If you notice that the validation error consistently goes up, what is likely going on? How can you fix this?
Kemungkinan terjadi **overfitting**. Solusinya adalah menggunakan **early stopping** atau teknik regularisasi (Ridge/Lasso), atau mengurangi jumlah epoch.

---

## 6. Is it a good idea to stop Mini-batch Gradient Descent immediately when the validation error goes up?
Tidak. Mini-batch Gradient Descent mengalami **fluktuasi alami**, jadi lebih baik gunakan **early stopping dengan patience**.

---

## 7. Which Gradient Descent algorithm (among those we discussed) will reach the vicinity of the optimal solution the fastest? Which will actually converge? How can you make the others converge as well?
**Stochastic Gradient Descent** biasanya mencapai solusi mendekati optimal lebih cepat, tapi fluktuatif. **Batch Gradient Descent** lebih stabil. Semua bisa dikonvergenkan dengan learning rate schedule atau adaptive learning rate.

---

## 8. Suppose you are using Polynomial Regression. You plot the learning curves and you notice that there is a large gap between the training error and the validation error. What is happening? What are three ways to solve this?
Itu tanda **overfitting**. Solusi:
- Kurangi derajat polinomial
- Gunakan lebih banyak data
- Terapkan regularisasi

---

## 9. Suppose you are using Ridge Regression and you notice that the training error and the validation error are almost equal and fairly high. Would you say that the model suffers from high bias or high variance? Should you increase the regularization hyperparameter α or reduce it?
Ini adalah gejala **underfitting**. Solusinya adalah **mengurangi regularisasi (α)** agar model lebih fleksibel.

---

## 10. Why use:
### a. Ridge Regression instead of plain Linear Regression (i.e., without any regularization)?
Untuk mengurangi overfitting dengan menambahkan regularisasi.

### b. Lasso instead of Ridge Regression?
Jika ingin **feature selection otomatis** karena Lasso mendorong beberapa koefisien menjadi nol.

### c. Elastic Net instead of Lasso?
Kombinasi Ridge dan Lasso. Digunakan jika jumlah fitur > jumlah sampel, atau fitur berkorelasi tinggi.

---

## 11. Suppose you want to classify pictures as outdoor/indoor and daytime/nighttime. Should you implement two Logistic Regression classifiers or one Softmax Regression classifier?
Gunakan **dua Logistic Regression classifier**, karena dua label tersebut **independen (multi-label classification)**, bukan eksklusif.




