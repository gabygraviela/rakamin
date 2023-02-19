# EDA Insight

## Data Numerik

### From boxplot and violin plot
- `city_development_index`:
  - Distribusi data city_development_index pada target 0 lebih kecil dibandingkan dengan target 1.
  - Median `city_development_index` berada diatas 0.9, yang artinya kebanyakan kandidat yang tidak sedang mencari perubahan pekerjaan berasal dari kota yang memiliki nilai `city_development_index` yang tinggi (kot-kota maju). Sedangkan, kandidat yang sedang mencari perubahan pekerjaan berasal dari kota dengan nilai `city_development_index` yang lebih rendah (median = 0.73).
  - Outliers hanya terdapat pada data kandidat yang tidak sedang mencari perubahan pekerjaan, dimana outliers berada dibawah nilai 0.64. Artinya, meskipun banyak dari mereka yang berasal dari kota besar, terdapat beberapa kandidat dari kota kecil yang juga tidak ingin mencari perubahan pekerjaan.

- `training_hours`:
  - Distribusi data pada kolom `training_hours` antara kandidat yang sedang mencari perubahan kerjaan dan yang tidak hampir sama. Kebanyakan kandidat menyelesaikan training dalam waktu kurang lebih 50 jam.
  - Pada umumnya, kandidat dapat menyelesaikan training dalam waktu 1 sampai 180 jam. Tapi ada beberapa persen orang yang tidak cukup mampu menyelesaikan training dalam jangka waktu tersebut (outlier), baik dalam kategori kandidat yang sedang mencari perubahan pekerjaan atau yang tidak.
  - Rekomendasi untuk tim bisnis: Lebih fokus pada kandidat dengan training hours diatas 180, karena semakin lama waktu training yang dibutuhkan, akan memerlukan cost yang lebih besar.

### From KDE Plot
- `city_development_index`:
  - Distribusi kolom `city_development_index` adalah bimodal karena terdapat dua lonjakan pada distribusi data.
  - Lonjakan terbesar berada di sekitar nilai indeks 0.9. Ini artinya kebanyakan kandidat yang mengikuti training adalah kandidat yang berasal dari kota-kota besar.
  - Namun, juga terdapat lonjakan di sekitar nilai indeks 0.62, yang menunjukkan bahwa jumlah kandidat dari kota yang tidak tergolong kota besar juga cukup banyak, walau tidak sebanyak kandidat yang berasal dari kota besar.

- `training_hours`
  - Distribusi data pada kolom `training_hours` adalah positively skewed.
  - Kebanyakan kandidat dapat menyelesaikan training dalam waktu 1-180 jam.
  - Tapi, terdapat data outliers, dimana data-data tersebut bernilai jauh lebih tinggi daripada data-data lainnya (dapat dilihat dari adanya pencilan pada kanan grafik).

## Data Kategorik
- Jumlah kandidat yang ingin mencari perubahan pekerjaan dengan pengalaman yg relevan dengan Data Science adalah sebesar 2.961, dengan persentase sebanyak 21.4%, sedangkan jumlah kandidat yang ingin mencari perubahan pekerjaan namun tidak memiliki pengalaman yang relevan dengan Data Science (switch career) adalah sebesar 3.550, dengan persentase sebanyak 66.1%. <br>
Rekomendasi bisnis : Perusahaan bisa meninjau ulang untuk membuat kandidat yang memiliki pengalaman yang relevan untuk switching career.
- Jumlah kandidat yang ingin mencari perubahan pekerjaan yang tidak berkuliah (bukan lulusan Universitas) relevan adalah sebesar 2.921, dengan persentase sebanyak 21.1%, sedangkan jumlah kandidat yang ingin mencari perubahan pekerjaan yang full time course (fokus kuliah saja) adalah sebesar 1.431, dengan persentase sebanyak 61.5%.<br>
Rekomendasi bisnis : persentase kandidat yang mencari perubahan pekerjaan bisa dinaikan dengan perusahaan dapat lebih mempromosikan benefit yang didapatkan dari training, salah satunya mendapatkan kesempatan dalam program penyaluran tenaga kerja perusahaan di bidang data scientist.
- Berdasarkan kolom city_development_index, kota dengan city development index sekitar 0.62 - 0.78 (kota kecil), memiliki proporsi kandidat yang ingin mencari perubahan pekerjaan cukup banyak dibanding dengan kandidat yang tidak ingin mencari perubahan pekerjaan. <br>
Rekomendasi bisnis : Perusahaan bisa lebih memperhatikan asal kota dari tiap kandidat yang mendaftar, karena kandidat yang berasal dari kota-kota kecil memiliki peluang untuk mencari perubahan pekerjaan.
- Dari data kolom training_hours, dapat dilihat bahwa mayoritas kandidat dapat menyelesaikan training dalam jangka waktu kurang lebih antara 1-180 jam. Tetapi, terdapat data-data outliers yang menunjukkan adanya kandidat yang membutuhkan waktu lebih dari 180 jam untuk menyelesaikan training. Lebih fokus pada kandidat dengan training hours diatas 180, karena semakin lama waktu training yang dibutuhkan, akan memerlukan cost yang lebih besar.<br> 
Rekomendasi bisnis : Perusahaan lebih memperhatikan dalam melakukan screening kelayakan kandidat untuk mengikuti training pada perusahaan, sehingga kandidat yang didapatkan adalah mereka yang benar-benar serius dan berpeluang lulus dalam waktu yang diharapkan.


# Business Insight
1. Jumlah kandidat yang ingin mencari perubahan pekerjaan dengan pengalaman yg relevan dengan Data Science adalah sebesar 2.961, dengan persentase sebanyak 21.4%, sedangkan jumlah kandidat yang ingin mencari perubahan pekerjaan namun tidak memiliki pengalaman yang relevan dengan Data Science (switch career) adalah sebesar 3.550, dengan persentase sebanyak 66.1%. Perusahaan bisa meninjau ulang untuk membuat kandidat yang memiliki pengalaman yang relevan untuk switching career.
2. Jumlah kandidat yang ingin mencari perubahan pekerjaan yang tidak berkuliah (bukan lulusan Universitas) relevan adalah sebesar 2.921, dengan persentase sebanyak 21.1%, sedangkan jumlah kandidat yang ingin mencari perubahan pekerjaan yang full time course (fokus kuliah saja) adalah sebesar 1.431, dengan persentase sebanyak 61.5%. 
3. Dari data kolom training_hours, dapat dilihat bahwa mayoritas kandidat dapat menyelesaikan training dalam jangka waktu kurang lebih antara 1-180 jam. Tetapi, terdapat data-data outliers yang menunjukkan adanya kandidat yang membutuhkan waktu lebih dari 180 jam untuk menyelesaikan training. Lebih fokus pada kandidat dengan training hours diatas 180, karena semakin lama waktu training yang dibutuhkan, akan memerlukan cost yang lebih besar.
4. Berdasarkan kolom city_development_index, kota dengan city development index sekitar 0.62 - 0.78 (kota kecil), memiliki proporsi kandidat yang ingin mencari perubahan pekerjaan cukup banyak dibanding dengan kandidat yang tidak ingin mencari perubahan pekerjaan

# Recomendation
1. Perusahaan bisa meninjau ulang untuk membuat kandidat yang memiliki pengalaman yang relevan untuk switching career.
2. Persentase kandidat yang mencari perubahan pekerjaan bisa dinaikan dengan perusahaan dapat lebih mempromosikan benefit yang didapatkan dari training, salah satunya mendapatkan kesempatan dalam program penyaluran tenaga kerja perusahaan di bidang data scientist.
3. Perusahaan lebih memperhatikan dalam melakukan screening kelayakan kandidat untuk mengikuti training pada perusahaan, sehingga kandidat yang didapatkan adalah mereka yang benar-benar serius dan berpeluang lulus dalam waktu yang diharapkan.
4. Perusahaan bisa lebih memperhatikan asal kota dari tiap kandidat yang mendaftar, karena kandidat yang berasal dari kota-kota kecil memiliki peluang untuk mencari perubahan pekerjaan.


 # Data Pre-Processing
 
 
