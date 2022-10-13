## PROJECT : Employee Analysis Attrition Report


### **Problem Statement**
Perusahaan memiliki 1.470 karyawan, ada sekitar 243 karyawan yang memutuskan resign dengan persentase 16% dan 1.233 karyawan masih bertahan di kantor dengan persentase 84%. Perusahaan perlu melakukan evaluasi terhadap karyawan yang resign terutama Departement Sumber Daya Manusia terutama bagian Human Resource Development sebagai evaluasi kedepan dalam mempertahankan karyawan untuk tidak resign dari kantor saat ini. Jika hal ini dibiarkan maka akan mengganggu produktivitas perusahaan terutama dalam menjalankan bisnisnya.

### **Objectives**
Hasil analisa ini akan memberikan insight dan saran kepada Departement Sumber Daya Manusia (Dept. SDM), dalam hal `karakteristik karyawan yang resign dari kantor dan faktor apa yang paling berpengaruh terhadap karyawan yang resign.`

### **Analytical Approach**
- Pendekatan analisa ini dengan cara melakukan pembagian variabel pada saat dilakukan Exploratory Data Analyst , Visualisasi Data dan Machine Learning :
  - Melakukan Exploratory Data Analyst terhadap seluruh variabel yang ada untuk mengetahui karakteristik karyawan yang resign dari kantor (Jupyter NoteBook).
  - Melakukan Visualisasi data dari setiap analisa untuk mendapatkan gambaran secara visual dari hasil Exploratory Data Analyst (Tableau).
  - Membuat model machine learning untuk mengetahui faktor apa yang paling berpengaruh terhadap keputusan karyawan untuk resign (Jupyter NoteBook).

| **Nama Kolom** | **Keterangan Kolom** |
| --- | --- |
|Age|Umur Karyawan yang bekerja di perusahaan|
|Gender|Jenis kelamin karyawan yang bekerja di perusahaan|
|Distance From Home|Jarak rumah karyawan ke perusahaan|
|Education|Pendidikan trakhir karyawan|
|Marital Status|Status pernikahan karyawan|
|Department|Departement karyawan bekerja|
|Job Role|Bidang pekerjaan karyawan|
|OverTime|Status karyawan lembur atau tidak|
|Business Travel|Keterangan karyawan melakukan perjalanan dinas atau tidak|
|Performance Rating|Peringkat performa perusahaan|
|Stock Option Level|Tingkat kepemilikan saham perusahaan|
|Job Involvement|Tanggung jawab karyawan dengan pekerjaan|
|Work Life Balance|Kesimbangan antara perkerjaan dengan kehidupan|
|Job Satisfaction|Hubungan pekerjaan karyawan|
|Relationship Satisfaction|Hubungan karyawan dengan rekan kerja|
|Enviroment Satisfaction|Hubungan karyawan dengan lingkungan kerja|
|Monthly Income|Pendapatan perbulan karyawan|
|Monthly Rate|Gaji perbulan karyawan|
|Daily Rate|Pendapatan harian karyawan|
|Hourly Rate|Pendapatan perjam karyawan|
|Percentage Salary Hike|persentase kenaikan gaji karyawan|
|Total Working Year|Total lama karyawn bekerja di perusahaan sebelumnya|
|Training Time Last Year|Tahun trakhir karyawan ikut pelatihan|
|Years At Company|Total karyawan berkerja di perusahaan sekarang|
|Years Since Current Role|Total tahun karyawan bekerja di posisi sekarang|
|Years Since Last Promotion|Total tahun karyawan dipromosikan|
|Years With Current Manager|Total tahun karyawan bekerja dengan manager|
|Num Companies Worked|Total perusahaan karyawan bekerja|

#### Columns Satisfaction
| **Num** | **Education** | **Num** | **EnvironmentSatisfaction** | **Num** | **JobInvolvement** | **Num** | **JobSatisfaction** | **Num** | **PerformanceRating** |
| --- | --- |--- | --- | --- | --- |--- | --- |--- | --- |
|1|Below College|1|Low|1|Low|1|Low|1|Low|
|2|College|2|Medium|2|Medium|2|Medium|2|Good|
|3|Bachelor|3|High|3|High|3|High|3|Excellent|
|4|Master|4|Very High|4|Very High|4|Outstanding| | |
|5|Doctor| | | | | | | | |
| **Num** | **RelationshipSatisfaction** | **Num** | **WorkLifeBalance** |  |  |  |  |  |  |
|1|Low|1|Bad| | | | | | |
|2|Medium|2|Good| | | | | | |
|3|High|3|Better| | | | | | |
|4|Very High|4|Best| | | | | | |

## DATA ANALYST
<hr>

### BASIC INFO :

##### AGE :

![a1](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Age%201.jpeg)

![a2](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Age%202.jpeg)

![a3](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Age%203.jpeg)

- Insight :
  - Perusahaan memiliki karyawan yang berumur paling kecil 18 tahun dan paling besar ada pada 60 tahun.
  - Jika dilihat dari hasil visualisasi Kernel Density Estimation (KDE) karyawan yang memilih resign paling banyak berada pada umur menjelang 30 tahun sampai dengan awal 30 tahun. Jika dilihat pada visualisasi bar plot banyak karyawan yang resign pada umur 29 tahun sampai dengan umur 31 tahun sedangkan untuk umur diatas 31 tahun banyak karyawan yang memilih untuk tetap tinggal di perusahaan.

##### GENDER :

![b1](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Gender%201.jpeg)

![a2](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Gender%202.jpeg)

![a3](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20Gender%203.jpeg)

- Insight :
  - Total karyawan dengan gender male ada 882 orang dengan persentase 60% dan karyawan dengan gender female ada 588 dengan persentase 40%.
  - Dari 60% gender male diperusahaan, ada 10,2% gender male resign dan dari 40% wanita gender female diperusahaan, ada 5,9% wanita memilih resign dari perusahaan.

##### DICTANCE FROM HOME

![c1](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20DistanceFromHome%201.jpeg)

![c2](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20DistanceFromHome%202.jpeg)

![c3](https://github.com/mhdalfarisy/Employee-Analysis-Attrition-Report/blob/main/a/Visualisasi%20DistanceFromHome%203.jpeg)

- Insight :
  - Jarak rumah karyawan dari kantor paling dekat ada pada 1 km dan paling jauh ada pada 29 km
  - Dari jarak terdekat yaitu 1 km dari rumah karyawan ke kantor sampai dengan jarak terjauh yaitu 29km ada karyawan yang resign namun jika dilihat dari keseluruhan karyawan yang resign tertinggi ada pada jarak kurang dari 10 km dari kantor dan jarak diatas 10 km mulai menurun tingkat karyawan resignnya. Jika dibandingkan dengan karyawan tidak resign, paling banyak karyawan tidak resign ada pada jarak kurang dari 10km jarak rumah ke kantor dan sedangkan jarak rumah karyawan di atas 10 km tingkat karyawan tidak resign lebih rendah dari pada karyawan resign, yang artinya semakin jauh jarak lokasi rumah karyawan dengan kantor maka semakin besar peluang karyawan untuk resign.
