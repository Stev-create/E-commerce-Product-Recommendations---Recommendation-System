# E-commerce-Product-Recommendations---Recommendation-System

<h3>Source Dataset: https://www.kaggle.com/cclark/product-item-data</h3>

## Overview

Rekomendasi produk ini dibuat berdasarkan content-based filtering menggunakan cosine similarity dan Jaccard similarity. Untuk ringkasan hasil terdapat di bawah ini, sedangkan untuk lengkapnya ada di notebook ini.

### Results

#### EDA

Dataset di atas, masih memiliki tag-tag HTML seperti `<br>,` `<b>,` `<lu>` dan lainnya. Itu kenapa dilakukannya juga pembersihan teks pada project ini. 

#### Cosine Similarity & Jaccard Similarity

Pada cosine similarity memiliki persamaan:

$$similarity = cos(\theta) = \frac{\vec{A}\cdot \vec{B}}{\left | A \right |\left | B \right |}$$

Sedangkan untuk Jaccard Similarity:

$$J(A,B) = \frac{\left | A\cap B \right |}{\left | A\cup B \right |}$$

Dari persamaan-persamaan di atas, seharusnya kita sudah menangkap bagaimana cosine dan Jaccard Similarity bekejar. Pada Cosine, semakin kecil sudutnya (bisa dibayangkan kedekatan dua objek) semakin besar nilainya. Sedangkan untuk Jaccard, semakin banyak irisannya semakin besar nilainya. 




