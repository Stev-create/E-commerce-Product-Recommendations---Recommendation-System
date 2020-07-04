# E-commerce-Product-Recommendations---Recommendation-System

<h3>Source Dataset: https://www.kaggle.com/cclark/product-item-data</h3>

## Overview

Rekomendasi produk ini dibuat berdasarkan content-based filtering menggunakan cosine similarity dan Jaccard similarity. Untuk ringkasan hasil terdapat di bawah ini, sedangkan untuk lengkapnya ada di notebook ini.

### Results

#### EDA

Dataset di atas, masih memiliki tag-tag HTML seperti `<br>,` `<b>,` `<lu>` dan lainnya. Itu kenapa dilakukannya juga pembersihan teks pada project ini. 

#### Cosine Similarity & Jaccard Similarity

Pada cosine similarity memiliki persamaan:
<center>
<a href="https://www.codecogs.com/eqnedit.php?latex=similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" title="similarity = \cos(\theta) = \frac{\vec{A}\cdot \vec{B}}{\left | A \right |\left | B \right |}" /></a>
 </center>
 
Sedangkan untuk Jaccard Similarity:
<center>
<a href="https://www.codecogs.com/eqnedit.php?latex=J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" title="J(A,B) = \frac{\left | A\cap B \right |}{\left | A\cup B \right |}" /></a>
</center>
Dari persamaan-persamaan di atas, seharusnya kita sudah menangkap bagaimana cosine dan Jaccard Similarity bekejar. Pada Cosine, semakin kecil sudutnya (bisa dibayangkan kedekatan dua objek) semakin besar nilainya. Sedangkan untuk Jaccard, semakin banyak irisannya semakin besar nilainya. 




