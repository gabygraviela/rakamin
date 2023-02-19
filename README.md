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


 # B. Data Pre-Processing
 ## A. Handling Missing Value
Dengan nilai konstan:
df['gender'] = df['gender'].fillna('Other')
df['major_discipline'].fillna('Other')
df['company_type'] = df['company_type'].fillna('Other')
Dengan nilai mode:
df['enrolled_university'].fillna(df['enrolled_university'].mode()[0], inplace=True)
df['education_level'].fillna(df['education_level'].mode()[0], inplace=True)
df['experience'].fillna(df['experience'].mode()[0], inplace=True)
df['company_size'].fillna(df['company_size'].mode()[0], inplace=True)
df['last_new_job'].fillna(df['last_new_job'].mode()[0], inplace=True)
 
## B. Handling Duplicated Data
Memeriksa apakah ada duplicated data di dataset dengan data kolom ‘enrollee_id’.

df.duplicated().sum()

Output: 0

Tidak ada duplikasi data dalam dataset HR Analytics.

## C. Handling Outliers
Ada dua cara untuk meng-handle outliers, antara lain:
z-score
IQR
Hasil  dari z-score tidak berbeda signifikan dengan data saat EDA dengan  df.describe():

## D. Handling Outliers
Mencari nilai IQR kolom 'city_development_index':

Q1 = np.percentile(df['city_development_index'], 25)
Q3 = np.percentile(df['city_development_index'], 75)
IQR = Q3 - Q1
IQR = 0.18000000000000005

Memisahkan nilai upper dan lower bound 'city_development_index' :
		lower_bound = Q1 - (1.5 * IQR)
upper_bound = Q3 + (1.5 * IQR)

outliers = df.loc[(df['city_development_index'] < lower_bound) | (df['city_development_index'] > upper_bound)]

df.loc[(df['city_development_index'] < lower_bound) | (df['city_development_index'] > upper_bound), 'city_development_index'] = np.nan

Output outliers pada kolom
'city_development_index':
df.isna().sum()

Drop NaN value pada kolom 'city_development_index' :
df = df.dropna(subset=['city_development_index'])
df.info()

Menggunakan code yang sama  dengan kolom 'city_development_index'
Output outliers pada kolom ‘training_hours’ :
df.isna().sum()

Drop NaN value pada kolom ‘training_hours’ :
df = df.dropna(subset=['training_hours'])
df.info()

Memeriksa hasil handling  outliers dengan IQR :
num = ['city_development_index', 'training_hours']
obj = ['city','gender', 'relevent_experience', 'enrolled_university',
       'education_level', 'major_discipline', 'experience', 'company_size', 'company_type',
       'last_new_job', 'experience_level', 'graduate']

for i in range(0, len(num)):
    plt.subplot(2,1, i+1)
    sns.kdeplot(x = df[num[i]], color='blue')
    plt.xlabel(num[i])

plt.tight_layout()

Memeriksa hasil handling  outliers dengan IQR :
df.describe()

## D. Feature Transformation
Karena distribusi dari ‘city_development_index’ dan ‘training_hours’ adalah skewed, maka digunakan normalisasi MinMaxScaler.

df['city_development_index_norm'] = MinMaxScaler().fit_transform(df['city_development_index'].values.reshape(len(df), 1))

df['training_hours_norm'] = MinMaxScaler().fit_transform(df['training_hours'].values.reshape(len(df), 1))

## E. Feature Encoding
Label Encoding : city, gender, relevent_experience, enrolled_university, education_level, experience, last_new_job, experience_level
df['city'] = df['city'].astype('category').cat.codes
df['gender'] = df['gender'].astype('category').cat.codes
df['relevent_experience'] = df['relevent_experience'].astype('category').cat.codes
df['enrolled_university'] = df['enrolled_university'].astype('category').cat.codes
df['education_level'] = df['education_level'].astype('category').cat.codes
df['experience'] = df['experience'].astype('category').cat.codes
df['last_new_job'] = df['last_new_job'].astype('category').cat.codes
df['experience_level'] = df['experience_level'].astype('category').cat.codes

One Hot Encoding: major_discipline, company_size, company_type, graduate
for cat in ['major_discipline','company_size','company_type','graduate']:
 	onehots = pd.get_dummies(df[cat], prefix=cat)
 	df = df.join(onehots)
  
## G. Handle Imbalance Class
Memeriksa  jumlah data pada target 
Menampilkan persentase masing-masing target dan class imbalance ratio

Berdasarkan ratio imbalance yang diperoleh yaitu 33% maka imbalance class termasuk dalam kategori Mild sehingga diperlukan handling terhadap class imbalance
Handling Class Imbalance dilakukan dengan 2 cara, yaitu:
Smote (oversampling)
Undersampling

Model Test - Oversampling
Accuracy (Test Set) : 0.87
Precision (Test Set) : 0.86
Recall (Test Set) : 0.88
F1-Score (Test Set) : 0.87
AUC : 0.87

Model Test - Undersampling
Accuracy (Test Set) : 0.78
Precision (Test Set) : 0.82
Recall (Test Set) : 0.72
F1-Score (Test Set) : 0.77
AUC : 0.78

Berdasarkan output disamping, nilai akurasi model yang paling baik diperoleh dari teknik imbalance oversampling (SMOTE).

## G. Feature Extraction
1. Membuat kolom experience_level
Untuk mengetahui kualifikasi dari tiap kandidat berdasarkan berapa tahun pengalaman di dunia kerja. Dapat dikategorikan menjadi beberapa level dan dibuat kolom baru experience_level untuk mempermudah analisis.
<1 = novice
1-5 = Advanced beginner
6-15 = Competent
16-20 = Proficient
>20 = Expert
Note:
Range dari setiap level dapat di-customize berdasarkan kebutuhan.

## H. Feature Selection
1. Drop Features
Drop kolom ‘enrollee_id’
‘city’
Kolom city bisa di-drop karena memiliki jumlah unique values yang tinggi. Namun, untuk sekarang city akan dimasukkan terlebih dahulu dan akan dinilai performanya. Kita ingin mengetahui perbedaan performa model jika kita include dan tidak include kolom city.
‘education_level’ dan ‘experience’
Sedangkan, kolom ‘education_level’ dan ‘experience’ juga memiliki kemungkinan untuk di-drop karena di bagian feature extraction, kita telah membuat kolom baru yang memberikan insight yang kita butuhkan berdasarkan 2 kolom ini. Tapi, sama dengan kolom city, kita akan tetap memasukkan kedua kolom ini dan diuji performa modelnya terlebih dahulu.
Notes:
Karena jumlah data dan feature dalam dataset ini termasuk sedikit, semua fitur (kecuali enrollee_id) akan digunakan untuk machine learning.Setelah proses modelling, dapat dilihat mana fitur yang penting dan mana yang tidak, sehingga fitur yang tidak penting dapat di-drop.

2. Membuat kolom Graduate (unique value 'yes' dan 'no')
Membedakan antara kandidat yang sudah lulus kuliah (graduate) atau yang tidak/belum kuliah (non-graduate). Berikut adalah beberapa alasan kenapa kita memerlukan feature ini dalam memilih kandidat job hiring:
Menyelesaikan gelar universitas dapat menandakan tingkat komitmen dan disiplin tertentu. Pemberi kerja mungkin melihat kandidat lulusan sebagai orang yang telah menunjukkan kemampuan untuk menetapkan dan mencapai tujuan, dan memiliki ketekunan untuk menyelesaikan program yang menantang.
Pendidikan universitas biasanya mencakup berbagai macam mata pelajaran yang memberikan dasar pengetahuan yang umum, seperti critical thinking, problem soling, communication dan research skill.
Secara umum, memiliki gelar seringkali menjadi syarat untuk pekerjaan data scientist level entry, meskipun hal ini dapat bervariasi tergantung pada perusahaan dan persyaratan pekerjaan tertentu.
Kolom yang digunakan adalah education_level dimana penggunaan unique value-nya pada kolom baru graduate adalah sebagai berikut:
'Graduate', 'Masters', 'Phd' = 'yes'
'Primary School' dan 'High School' = 'no'

## I. Additional Feature
Unemployment Duration
Jika diberikan kesempatan untuk bekerja sebagai data scientist, orang yang telah menganggur dalam waktu yang lama pasti akan tertarik untuk mengambil kesempatan ini dan beralih profesi.
Salary
Jika kita menawarkan gaji sebesar xxx, maka kemungkinan orang yang saat ini menerima gaji di bawah jumlah tersebut akan lebih tinggi untuk mempertimbangkan perubahan pekerjaan.
Relevance between current job and major discipline
Orang yang memiliki latar belakang pekerjaan di luar disiplin ilmu STEM atau disiplin ilmu yang relevan dengan bidang data science berkemungkinan tinggi untuk mempertimbangkan beralih profesi ke bidang data science jika diberikan kesempatan dalam program data scientist hiring.
Age
Orang yang telah memasuki usia tua cenderung kurang berminat untuk mengganti pekerjaan lagi. Alasannya bisa berupa:
Sudah memiliki pengalaman dan keterampilan pada bidang pekerjaannya sekarang yang telah dikembangkan bertahun-tahun.
Sudah nyaman dengan perusahaan yang sekarang dan cenderung merasa sulit untuk beradaptasi dengan work culture yang baru.








