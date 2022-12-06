# **TEMA     : KLASIFIKASI KUALITAS LEMON🍋**
---
### Table of Contents

* [Anggota Kelompok](#chapter1)
* [About Dataset](#chapter2)
* [About Project](#chapter3)
* [Data Collecting](#chapter4)
* [Data Preprocessing](#chapter5)
* [Data Visualisasi & Analysis](#chapter6)
* [Modelling](#chapter7)
* [Prediksi](#chapter8)
* [Download Dataset](#chapter9)
* [Download Model](#chapter10)

---
# **KELOMPOK : 5 A2** <a class="anchor" id="chapter1"></a>
1.   **2009106026 SULHAIRAH** (Data Modelling & Evaluasi)
2.   **2009106028 MITHA AMALIA** (Data Collecting & Preprocessing)
3.   **2009106030 PATRICIA CHANDRA** (Visualisasi & Confuision Matrix)

# **LINK Download Model** <a class="anchor" id="chapter10"></a>
Link Model : https://drive.google.com/drive/folders/1Dn7n9MNKAfWLZdpVDr4388Ue7VkquqI0?usp=share_link

# **LINK Download Dataset** <a class="anchor" id="chapter9"></a>
Link dataset awal : https://drive.google.com/drive/folders/1E19JJB3Fgi17nAW36ISpRJE5TVFzhO0e?usp=share_link
<br>Link dataset split folder : https://drive.google.com/drive/folders/1vZV1c5IS9o9p2FC0qTE5zL6aYOUF0Qpc?usp=share_link

# **ABOUT DATASET** <a class="anchor" id="chapter2"></a>
Lemon dataset telah disiapkan untuk menyelidiki kemungkinan untuk mengatasi masalah kontrol kualitas buah. Ini berisi 2040 gambar (300 x 300 piksel). Gambar lemon diambil pada permukaan beton. Dataset berisi gambar lemon berkualitas buruk dan baik di bawah kondisi pencahayaan yang sedikit berbeda (semua di bawah sinar matahari).


# **ABOUT PROJECT** <a class="anchor" id="chapter3"></a>
Project ini mendeteksi kualitas lemon dalam kategori baik atau buruknya lemon dengan gambar, berdasarkan dataset dan luar dataset.

# **DATA COLLECTING** <a class="anchor" id="chapter4"></a>
Dalam data collecting tempat menyimpan database terdapat dalam google drive.
-	Gambar yang bad quality berjumlah 951 gambar
-	Gambar yang good quality berjumlah 1125 gambar
-	Ukuran dari kualitas gambar adalah 300,300, 3

Berikut adalah contoh kualitat lemon yang buruk dari dataset:

| Bad Quality | Good Quality |
| ------------ | ------------- |
| <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/coleccting.PNG" width="250"> | <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/collectinggood.PNG" width="250">|


# **DATA PREPROCESSING** <a class="anchor" id="chapter5"></a>
**TRAINING**
-	Pada training terdapat rescale dimana untuk mempercepat training
-	Horizontal flip untuk membaca gambar jika dalam keadaan terbalik
-	Juga terdapat pengaturan brightness mendeteksi jika gambar redup atau terang nantinya
-	Zoom range untuk memperbesar gambar di sini kami mengatur perbesar zoomnya hanya dua kali.
-	Target sizenya 150, 150 untuk merubah dimensi ke 150,150
-	Batch size 64
-	Class mode menggunakan binary karena pernyataan yang diinginkan hanyalah good atau bad.
VALIDATION
-	Pada validasi ini terdapat target size, batch dan class mode seperti yang digunakan sebelumnya pada training
TEST
-	Pada test ini terdapat target size, batch dan class mode seperti yang digunakan sebelumnya pada training

# **DATA VISUALISASI & ANALYSIS** <a class="anchor" id="chapter6"></a>
Menampilkan gambar hasil augmentasi dengan ukuran pada setiap gambar 64, 150, 150, 3. Di sini menggunakan temp untuk mengubah float menjadi int indeks karena sebelumnya masih float (float tidak bisa digunakan).
Gambar akan muncul sebagai berikut:

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/data%20visualisasi.PNG" />
</p>

**TRAINING**
-	Pada training terdapat rescale dimana untuk mempercepat training
-	Horizontal flip untuk membaca gambar jika dalam keadaan terbalik
-	Juga terdapat pengaturan brightness mendeteksi jika gambar redup atau terang nantinya
-	Zoom range untuk memperbesar gambar di sini kami mengatur perbesar zoomnya hanya dua kali.
-	Target sizenya 150, 150 untuk merubah dimensi ke 150,150
-	Batch size 64
-	Class mode menggunakan binary karena pernyataan yang diinginkan hanyalah good atau bad.
**VALIDATION**
-	Pada validasi ini terdapat target size, batch dan class mode seperti yang digunakan sebelumnya pada training
**TEST**
-	Pada test ini terdapat target size, batch dan class mode seperti yang digunakan sebelumnya pada training

**Jumlah Dataset Train, Test, dan Val**
Berikut adalah jumlah gambar dataset keseluruhan, kualitas lemon dan jumlah data dibedakan menjadi dua warna.
<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/Jumlah%20Gambar%20Dataset%20Keseluruhan.png" />
</p>

**Jumlah Data Train**
Berikut adalah jumlah gambar dataset Train, kualitas lemon dan jumlah data dibedakan menjadi dua warna.

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/Jumlah%20Gambar%20Dataset%20Train.png" />
</p>

**Jumlah Data Test**
Berikut adalah jumlah gambar dataset Test, kualitas lemon dan jumlah data dibedakan menjadi dua warna.

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/Jumlah%20Gambar%20Dataset%20Test.png" />
</p>

**Jumlah Data Validation**
Berikut adalah jumlah gambar dataset validation, kualitas lemon dan jumlah data dibedakan menjadi dua warna.

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/Jumlah%20Gambar%20Dataset%20Validation.png" />
</p>

**Classification report dan Confusion Matrix**
Berikut terlihat hasil confusion matrix dan classification matrix berdasarkan hasil dari data set. Berikut gambarnya: 

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/confuison.PNG" />
</p>

# **MODEL** <a class="anchor" id="chapter7"></a>
  Model yang kami gunakan di sini adalah image processing dengan alogaritma CNN.  Di sini kami menggunakan activation relu sebagai hidden layer dan sigmoid sebagai output layers.  
-	Model compile loss = 'binary_crossentropy' dikarenakan output hanya dua
-	optimizer='rmsprop', menggunakan rmsprop dikarenakan akurasi lebih tinggi dari adam (telah dicoba)
-	metrics=['accuracy'],  digunakan untuk mencari akurasi.
**Evaluate**
Dan berikut adalah gambar akurasi dari evaluate model: 

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/Evaluate.PNG" />
</p>

# **PREDIKSI** <a class="anchor" id="chapter8"></a>
Memprediksi gambar lemon bad atau good. Menampilkan actual dan hasil prediksi dari masing- masing gambar dalam dataset. Berikut gambarnya:

<p align="center">
  <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/prediksi.PNG" />
</p>

Memprediksi gambar yang dinputkan secara manual atau satu persatu. Berikut adalah gambarnya: 

| Bad Quality | Good Quality |
| ------------ | ------------- |
| <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/prediksibad.PNG" width="250"> | <img src="https://github.com/Mithaamalia13/PA_KB_5_A2-20/blob/main/prediksigood.PNG" width="250">|
