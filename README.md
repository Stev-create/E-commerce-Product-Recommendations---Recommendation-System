# E-commerce-Product-Recommendations---Recommendation-System

<h3>Source Dataset: https://www.kaggle.com/cclark/product-item-data</h3>

## Overview

Rekomendasi produk ini dibuat berdasarkan <i>content-based filtering</i> menggunakan dua pendekatan yaitu <b>Cosine Similarity dan Jaccard Similarity.</b> Kemudian saya akan coba bandingkan keduanya secara kualitatif. Untuk ringkasan hasil terdapat di bawah ini, sedangkan untuk lengkapnya ada di [notebook ini](https://github.com/Stev-create/E-commerce-Product-Recommendations---Recommendation-System/blob/master/E-Commerce%20Product%20Recommendation.ipynb).

### Results

#### EDA

Dataset di atas, masih memiliki tag-tag HTML seperti `<br>`, `<b>`, `<ul>` dan lainnya. Itu kenapa dilakukannya juga pembersihan teks pada project ini. Kemudian jumlah karakter di dataset ini relatif sedikit, mengingat fitur di dataset ini hanya satu, yaitu deskripsi produk. Yang distribusinya dapat dilihat di bawah:

![GitHub Logo](/images/1.png)

Produk-produk di dataset ini kebanyakan produk untuk pakaian luar. Itu kenapa, kata-kata yang bermunculan adalah kata-kata yang berhubungan dengan bahan-bahan baju dan ramah lingkungan. Yang words cloudnya dapat di lihat di bawah:

![GitHub Logo](/images/2.png)

#### Cosine Similarity & Jaccard Similarity

Cosine Similarity punya persamaannya yang sederhana, yaitu:

<a href="https://www.codecogs.com/eqnedit.php?latex=similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" title="similarity = \cos(\theta) = \frac{\vec{A}\cdot \vec{B}}{\left | A \right |\left | B \right |}" /></a>
 
Sedangkan untuk Jaccard Similarity:

<a href="https://www.codecogs.com/eqnedit.php?latex=J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" title="J(A,B) = \frac{\left | A\cap B \right |}{\left | A\cup B \right |}" /></a>

Dari persamaan-persamaan di atas, seharusnya kita sudah menangkap bagaimana Sosine dan Jaccard Similarity bekerja. Pada Cosine, semakin kecil sudutnya (bisa dibayangkan kedekatan dua objek) semakin besar nilainya. Sedangkan untuk Jaccard, semakin banyak irisannya (atau miripnya) semakin besar nilainya. 

## Conclusion

Pada sistem rekomendasi memang tidak ada sistem yang lebih baik atau lebih buruk. Namun kalau dilihat dari hasil antara dua pendekatan di atas, mereka memiliki hasil yang bersinggungan dan rekomendasi-rekomendasi yang diberikan mirip dengan produk yang dipilih. Hasilnya dapat dilihat di [notebook ini](https://github.com/Stev-create/E-commerce-Product-Recommendations---Recommendation-System/blob/master/E-Commerce%20Product%20Recommendation.ipynbm), bagian terakhir (<i>sanity check</i>).





