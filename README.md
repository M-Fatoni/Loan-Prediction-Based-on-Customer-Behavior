## Descriptive Analysis
Terdapat 13 kolom yang dimiliki pada dataset ini yaitu Id, Income, Age, Experience, Married/Single, House Ownership, Car Ownership, Profession, City, State, Current Job Years, Current House Years, dan Risk Flag. Tidak terdapat missing data dan duplikat pada dataset ini sehingga tidak perlu dilakukan imputasi data.
Langkah pertama yang perlu dilakukan adalah untuk menghapus kolom Id dikarenakan hanya merupakan identitas dari tiap peminjam sehingga tidak memberikan value apapun pada feature lainnya. Pada fitur lain, tidak terlihat adanya keanehan dalam data. Perbedaan jumlah nilai dari masing-masing fitur pun cukup tersebar secara merata namun ketimpangan hanya terjadi pada kolom Married/Single, House Ownership, Car Ownership, dan Risk Flag.

## Univariate Analysis
Pada kolom umur tidak terlihat pola sama sekali, 3 umur tertinggi peminjam adalah 27, 66, dan 48. Namun ketika kolom umur dikelompokan berdasarkan umur dibawah 30, 40, 50, 60, dan pensiun, terlihat peminjam yang sudah pensiun memiliki nilai yang lebih besar dibandingan rentang usia lain.
Pada kolom income, data sudah terdistribusi secara uniform sehingga tidak diperlukan adanya proses lebih lanjut. Pada kolom pengalaman kami membagi menjadi "New", "New Intermediate", "Intermediate Advance", dan "Advance". Dari pengelompokan tersebut pengalaman pekerja yang baru memiliki nilai yang lebih tinggi dibanding kelompok pengalaman yang lain. Pada kolom pekerjaan, peminjam yang memiliki basic engineering merupakan peminjam terbanyak dibandingkan basic pekerjaan yang lain. Sementara pada kolom-kolom lainnya tidak terdapat perubahan pola yang cukup signifikan.

## Multivariate Analaysis:
Dari Visualisasi Heatmap, Terlihat bahwa fitur CURRENT_JOB_YRS dan Experience memiliki korelasi yang tinggi.
Dengan menggunakan chi square test, fitur yang memiliki korelasi dengan Risk_Flag adalah Car_Ownership.
Dengan menggunakan Metode Anova dan Pearson Correlation, Experience lah yang memiliki korelasi dengan Risk_Flag.
Dari matriks korelasi antar fitur, tidak ada pola yang menarik yang terlihat. Hal ini menunjukkan bahwa tidak ada hubungan kuat antara fitur-fitur numerik tersebut. Oleh karena itu, tidak diperlukan tindakan khusus terhadap fitur-fitur numerik ini. fitur-fitur yang tidak memiliki korelasi kuat dengan Risk_Flag juga tidak perlu dibuang untuk saat ini karena walaupun kecil, masih ada sedikit informasi di dalamnya yang mungkin bisa digunakan nantinya.

Namun, dari uji chi-square dan ANOVA, kita melihat bahwa Car_Ownership dan Experience memiliki hubungan yang signifikan dengan label (Risk_Flag). Ini berarti bahwa kepemilikan mobil dan pengalaman dapat menjadi faktor yang relevan dalam memprediksi risiko gagal bayar. Oleh karena itu, fitur Car_Ownership dan Experience mungkin perlu dipertimbangkan lebih lanjut dalam model prediksi risiko gagal bayar.

Secara umum, hasil analisis menunjukkan bahwa faktor-faktor seperti status perkawinan, kepemilikan rumah, profesi, serta lokasi geografis dapat berpengaruh terhadap risiko pembayaran pinjaman.

Dari faktor-faktor ini dapat membantu lembaga keuangan untuk mengidentifikasi, mengukur, dan mengelola risiko pembayaran pinjaman dengan lebih efektif, serta mengambil keputusan yang lebih baik dalam hal penentuan kebijakan kredit dan pengelolaan risiko.

### Business Insight:
1. *Pendapatan dan Risiko Default*: Meskipun distribusi pendapatan pelanggan cenderung seragam, kelompok pelanggan yang mengalami default memiliki variasi pendapatan yang lebih besar dibandingkan dengan yang tidak mengalami default. Hal ini mengindikasikan bahwa keberagaman kondisi keuangan pelanggan yang mengalami default dapat menjadi faktor risiko yang penting dalam menentukan kemungkinan default.

2. *Usia dan Risiko Default*: Kelompok pelanggan yang mengalami default cenderung memiliki usia yang lebih muda daripada yang tidak mengalami default. Meskipun perbedaan rata-rata usia tidak signifikan, hal ini menunjukkan bahwa segmentasi berdasarkan usia dapat menjadi pertimbangan penting dalam menilai risiko kredit.

3. *Pengalaman Profesional dan Risiko Default*: Meskipun distribusi pengalaman profesional relatif merata, pelanggan yang tidak mengalami default cenderung memiliki pengalaman profesional yang lebih besar dibandingkan dengan yang mengalami default. Pengalaman profesional yang lebih panjang dapat mencerminkan stabilitas pekerjaan dan finansial, yang dapat mengurangi risiko default.

4. *Kepemilikan Rumah dan Mobil*: Pelanggan yang memiliki rumah sewa cenderung lebih berisiko default dibandingkan dengan yang tidak memiliki rumah sewa atau memiliki rumah sendiri. Sementara itu, pelanggan yang memiliki mobil memiliki risiko default yang lebih rendah dibandingkan dengan yang tidak memiliki mobil. Faktor-faktor ini dapat menjadi pertimbangan penting dalam penilaian risiko kredit.

### Business Recommendations:

1. *Segmentasi Pelanggan*: Lebih lanjut segmentasikan pelanggan berdasarkan faktor-faktor seperti usia, pengalaman profesional, kepemilikan rumah, dan mobil untuk memahami kecenderungan dan risiko kredit dengan lebih baik.

2. *Penilaian Risiko yang Lebih Dalam*: Lakukan penilaian risiko yang lebih dalam dengan mempertimbangkan faktor-faktor seperti variasi pendapatan, stabilitas pekerjaan, dan kepemilikan aset untuk mengidentifikasi pelanggan yang berisiko tinggi.

3. *Peningkatan Keamanan Kredit*: Tingkatkan keamanan kredit dengan memperketat persyaratan kredit untuk pelanggan dengan risiko tinggi, seperti mereka yang memiliki pendapatan yang bervariasi atau pengalaman profesional yang kurang stabil.

4. *Edukasi Keuangan*: Sediakan program edukasi keuangan untuk pelanggan yang berisiko, terutama mereka yang masih muda atau belum memiliki pengalaman profesional yang cukup, untuk membantu mereka mengelola keuangan mereka dengan lebih baik dan menghindari risiko default.

5. *Promosi Produk yang Sesuai*: Sesuaikan penawaran produk dan layanan dengan kebutuhan dan profil risiko pelanggan, seperti menawarkan program kredit yang lebih aman kepada pelanggan dengan risiko tinggi atau mengembangkan program kepemilikan rumah untuk membantu pelanggan menyewa rumah mereka sendiri.

6. *Penggunaan Pengalaman Profesional dan Kepemilikan Mobil sebagai Indikator Risiko*: Fokuskan analisis risiko kredit pada pengalaman profesional dan kepemilikan mobil sebagai indikator utama dalam menilai risiko default pelanggan.