# <font color = 'green'> Loan Prediction Based on Customer Behavior </font>

## <font color = 'darkgreen'> Chapter 1 </font>

## A. Role

Sebagai tim Data Scientist menggunakan pengetahuan dan keterampilan analisis data untuk memahami tren dan pola dalam dataset pinjaman. Bertanggung jawab untuk mengembangkan model prediksi yang dapat mengidentifikasi pelanggan yang berisiko default pada pinjaman berdasarkan fitur-fitur seperti pendapatan, usia, pengalaman, dan karakteristik lainnya. Selain itu, Data Scientist juga bertugas untuk menganalisis faktor-faktor yang mempengaruhi risiko default dan menghasilkan wawasan yang berguna bagi tim manajemen atau tim pengambil keputusan dalam mengelola portofolio pinjaman. Dengan menggunakan pendekatan analisis data dan teknik machine learning, Data Scientist berperan dalam membantu perusahaan atau institusi keuangan mengoptimalkan keputusan kredit dan mengurangi risiko gagal bayar dalam portofolio pinjamannya.

## B. Problem Statement

### Summary of The Problem

Organisasi ingin memprediksi pelanggan yang berpotensi mangkir untuk produk pinjaman konsumen berdasarkan data perilaku pelanggan historis yang mereka amati. Dengan demikian, mereka dapat mengidentifikasi pelanggan baru yang lebih berisiko dan mengambil tindakan proaktif untuk mengelola risiko default.

### Supporting Facts

- Menurut laporan industri keuangan, risiko default pelanggan dapat menyebabkan kerugian besar bagi perusahaan, terutama jika tidak dideteksi secara dini.
- Penelitian menunjukkan bahwa menggunakan teknik analisis data dan machine learning dapat membantu mengidentifikasi pola dan tren yang berkaitan dengan risiko default pelanggan.

### Problem Statement

- Menentukan apakah seorang pelanggan berisiko default pada pinjaman berdasarkan perilaku dan karakteristiknya.
- Membuat model prediksi untuk mengidentifikasi pelanggan yang berpotensi gagal membayar pinjaman.
- Menganalisis faktor-faktor yang mempengaruhi risiko default pada pinjaman.
- Menentukan apakah ada korelasi antara variabel seperti pendapatan, usia, atau pengalaman dengan risiko default pada pinjaman.

## C. Goal And Objective

### Goal 

Mengurangi risiko gagal bayar dalam portofolio pinjaman dan meningkatkan kualitas keputusan kredit dengan menggunakan analisis data dan model prediksi.

### Objectiveness

- Membangun model prediksi yang dapat mengidentifikasi pelanggan yang berpotensi default pada pinjaman dengan akurasi tinggi.
- Meningkatkan pemahaman tentang faktor-faktor yang mempengaruhi risiko default melalui analisis data yang mendalam.
- Mengoptimalkan keputusan kredit dengan menggunakan model prediksi untuk menilai risiko default pada setiap aplikasi pinjaman.
- Mengurangi kerugian finansial dan meningkatkan kepercayaan pelanggan dengan mengelola risiko default secara proaktif.

## D. Business Metrics

- `Rasio Default Pinjaman Konsumen`: Persentase dari total pinjaman konsumen yang gagal bayar dalam portofolio pinjaman. Metric ini membantu dalam melacak apakah jumlah pelanggan yang mangkir berkurang sesuai dengan tujuan untuk mengurangi risiko gagal bayar.
- `Tingkat Akurasi Model Prediksi`: Persentase dari prediksi model yang benar dari total prediksi yang dilakukan oleh model. Metric ini membantu dalam mengevaluasi seberapa baik model dapat mengidentifikasi pelanggan yang berpotensi mangkir dengan akurat.
- `Presisi dan Recall Model`: Persentase presisi (positif prediksi yang benar) dan recall (kasus positif yang diidentifikasi) dari model prediksi. Metric ini membantu dalam mengevaluasi seberapa baik model dapat mengelola risiko mangkir dengan mengoptimalkan jumlah pelanggan yang benar-benar berisiko mangkir dan meminimalkan jumlah pelanggan yang tidak terdeteksi sebagai berisiko mangkir.
- `Peningkatan Pendapatan Pinjaman`: Metric ini membantu dalam mengevaluasi dampak positif dari berkurangnya total pinjaman konsumen yang gagal bayar.

## <font color = 'darkgreen'> Chapter 2 </font>

## A. EDA

![Univariate](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/univariate.JPG)

![Bivariate 1](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate1.JPG)

![Bivariate 2](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate2.JPG)

![Bivariate 3](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate3.JPG)

![Bivariate 4](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate4.JPG)

![Bivariate 5](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate5.JPG)

![Bivariate 6](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate6.JPG)

![Bivariate 7](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/bivariate7.JPG)

![Multivariate](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/multivariate.JPG)

## B. Pemodelan Machine Learning

![ML Model Performance Comparison](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/ml.JPG)

![Random Forest Model](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/rf.JPG)

![Features Importance](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/feature_importance.JPG)

## C. Assumption Calculation (Repayment Rate)

![Assumption Calculation](https://github.com/M-Fatoni/LoanPrediction/blob/main/img/assumption.JPG)

## <font color = 'darkgreen'> Chapter 3 </font>

##  A. Business Recommendation

**1. Segmentasi Usia dan Penyesuaian Strategi:**

Fokus pada kelompok usia produktif (21-35 tahun) untuk memberikan perhatian 
khusus dalam pemantauan dan manajemen risiko, sementara memberikan 
penawaran khusus kepada kelompok usia lanjut (66-79 tahun) yang memiliki 
risiko gagal bayar yang lebih rendah. 

**2. Penilaian Status Perkawinan dan Kepemilikan Rumah:**

Bisnis dapat memberikan perhatian khusus pada individu yang status perkawinannya 
single dan mereka yang tinggal di rumah sewa, karena cenderung memiliki risiko gagal 
bayar yang lebih tinggi. Ini dapat mencakup penyesuaian tingkat bunga atau 
persyaratan lainnya untuk mengurangi risiko kredit.  

**3. Evaluasi Regional:**

Bisnis harus mempertimbangkan faktor regional dalam menilai risiko kredit. Negara 
bagian seperti Manipur, Tripura, dan Kerala memiliki risiko gagal bayar yang tinggi, 
sementara kota seperti Bhubaneswar memiliki risiko yang lebih tinggi dibandingkan 
dengan wilayah lainnya. Strategi pemasaran dan pengelolaan risiko harus disesuaikan 
dengan kondisi regional yang spesifik. 

**4. Optimasi Fitur dan Pengembangan Model:**

Fokus pada fitur-fitur yang paling signifikan seperti pendapatan, usia, dan lokasi 
dapat membantu meningkatkan akurasi prediksi dan pengelolaan risiko secara 
keseluruhan.


##  B. Conclussions

- Analisis data pelanggan menunjukkan bahwa faktor-faktor seperti 
usia, pendapatan, pengalaman, status perkawinan, state, kota, dan 
kepemilikan rumah berpengaruh signifikan terhadap risiko kredit. 

- Rekomendasi bisnis meliputi segmentasi pelanggan yang lebih tepat 
dan penerapan strategi pemberian pinjaman yang lebih cerdas 
berdasarkan prediksi risiko kredit menggunakan model Machine 
Learning, sehingga dapat mengurangi risiko pinjaman dan 
meningkatkan tingkat pembayaran kembali.


## <font color = 'darkgreen'> ThankYou </font>


```python

```
