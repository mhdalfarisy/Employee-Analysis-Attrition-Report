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

### **Kesimpulan Exploratory Data Analyst**

#### Basic Info :
  1. `Age :` Karyawan yang bekerja di perusahaan berumur paling rendah 18 tahun dan paling tinggi 60 tahun, dari keseluruhan umur karyawan yang paling banyak resign mulai dari umur 29 tahun sampai umur 31 tahun.
  2. `Gender:` Total karyawan berjenis kelamin pria (60%) lebih banyak dibandingkan karyawan wanita (40%) dan untuk karyawan yang resign paling banyak adalah pria dengan persentase 10,2%.
  3. `Distance From Home :` Jarak rumah karyawan ke kantor mulai dari 1 km sampai dengan 29km dan untuk karyawan yang paling banyak resign yang jarak rumahnya lebih dari 10km.
  4. `Education :` Perusahaan memiliki karyawan dengan pendidikan bacher 69,7% lebih banyak dibandingkan karyawan baground master dan doctor, berdasarkan pendidikan karyawan yang memiliki pendidikan bachelor lebih cenderung resign.
  5. `Marital Status :` Perusahaan memiliki karyawan paling banyak yang berstatus single lebih banyak 45,8% dan karyawan yang resign juga paling banyak berstatus single sebanyak 8,2% yang resign.
### Work Info :
  7. `Departement : ` Total karyawan pada department Sales 446 karyawan, department Research & Development 961 dan department Human Resources 63 orang dan karyawan yang paling banyak resign dari department Research & Development 9,0%.
  8. `Job Role : ` Banyak karyawan yang resign dari Job Role Laboratory Technician sebanyak 4,2%.
  9. `Over Time : ` Karyawan yang bekerja lembur sebanyak 416 orang dengan persentase 28,3% dan yang tidak bekerja lembur 1.054 dengan persentase 71,7% namun dari 28,3% karyawan memilih resign banyak dari yang bekerja lembur dengan persentase 8,6%.
  10. `Business Travel : ` Karyawan yang resign banyak berasal dari karyawan yang jarang melakukan perjalanan dinas sebanyak 156 orang dengan persentase 10,6%.
  11. `Perfomance Rating : ` Karyawan yang resign dari perusahaan banyak berasal dari karyawan yang memiliki performa bagus sebanyak 13,6% namun karyawanyang memiliki perfoma bagus yang tetap menentap diperusahaan lebih banyak 71,0%.
  12. `Stock Option Level : ` Karyawan yang resign paling banyak yang tidak mendapatkan saham perusahan sebanyak 10,5%, sedangkan karyawan yang mendapatkan saham perusahaan lebih banyak memilih menetap diperusahaan.
  13. `Job Involvement : ` Karyawan dengan tanggung jawab yang rendah paling banyak resign sedangkan karyawan yang paling sedikit resign pada karyawan yang memiliki tanggung jawab yang tinggi.
#### Satiscfaction :
  15. `Worklifebalance : ` Banyak karyawan yang masih bekerja di perusahaan karena mandapatkan work life balance yang tinggi dibandingkan karyawan yang resign memiliki work life balance yang rendah.
  16. `Job Satiscfaction: ` Banyak karyawan yang memiliki kepuasan bekerja sangat tinggi sebanyak 459 karyawan dengan persentase 31,2% dan memilih bertahan diperusahaan sedangkan karyawan yang memiliki persentase kerja yang rendah memilih  resign dari perusahaan.
  17. `Relationship Satisfaction : ` Rekan kerja yang memiliki hubungan baik dengan rekan kerja memiliki persentase tertinggi untuk resign dibandingkan rekan kerja yang memiliki hubungan dengan kerja yang rendah.
  18. `Environtment Employee`, Karyawan yang banyak resign berasal dari lingkungan kerja yang kurang nyaman (rendah), sedangkan karyawan yang memiliki lingkungan kerja yang bagus cenderung memilih bertahan di perusahaan.
#### Salary Related :
  20. `Monthly Income :` Karyawan cenderung resign jika perndapatan perbulan mereka dibawah 5000USD, sedangkan karyawan yang perndapatan perbulan diatas 5000USD lebih cenderung bertahan di perusahaan. 
  21. `Monthly Rate :` Karyawan cenderung resign pada gaji 10000USD sampai dengan dibawah 15000USD.
  22. `Daily Rate: ` Karyawan cenderung resign jika hitungan upah harian mereka dibawah 500USD.
  23. `Hourly Rate :` Banyak karyawan yang resign pada bayaran perjam mereka sekitar 40USD sampai dengan kurang dari 80USD.
  24.  `Percent Salary Hike :` Banyak karyawan yang resign jika kenaikan gaji mereka di bawah 10% dan karyawan yang memiliki kenaikan gaji diatas 10% lebih banyak memilih bertahan di perusahaan.
#### Time Related :
  25.  `Total Working Years :` Banyak karyawan yang resign dari pengalaman yang kurang dari 10 tahun bekerja.
  26.  `Training Time Last Year :` Karyawan yang paling banyak resign jika pada mereka yang belum pernah sama sekali mendapatkan training.
  27.  `Years at Company :` Banyak karyawan yang resign dari perusahaan yang kurang dari 10 tahun bekerja di perusahaan ini.
  28.  `Years In Current Role : ` Banyak karyawan yang resign dengan posisi sekarang kurang dari 5 tahun.
  29.  `Years Since Last Promotion :` Karyawan yang resign banyak dari yang belum dapat promosi, sedangkan karyawan yang sudah mendapatkan promosi cenderung memilih untuk bertahan di perusahaan.
  30.  `Years With Current Manager :` Karyawan banyak yang resign yang belum pernah sama sekali bekerja dengan manager, sedangkan karyawan yang sudah pernah bekerja dengan manager cenderung untuk bertahan di perusahaan.
  31.  `Num Companies Worked : ` Karyawan yang bekerja dari perusahaan sebelumnya ada dari yang fresh graduate sampai dengan sudah 9x bekerja di perusahaan yang berbeda, namun karyawan yang paling banyak resign ada pada yang bekerja sudah pada lebih dari 5 perusahaan.

## **Saran Exploratory Data Analyst**

#### Basic Info :
  -  Perusahaan perlu memfokuskan karyawan yang menuju umur 30 tahun berpendidikan bachelor baik itu laki-laki ataupun perempuan yang masih single terutama yang jarak rumahnya lebih 10 km dari kantor.
### Work Info :
  - Karyawan dari department Research & Development terutama yang bekerja sebagai Laboratory Technician perlu dievaluasi sistem jam kerjanya untuk menghindari karyawan sering bekerja overtime. terutama karyawan yang memiliki performa kerja yang bagus.
  - Untuk Karyawan yang sudah berkontribusi lebih dari 10 tahun perusahaan dengan performa yang bagus dan bertanggung jawab maka perusahaan dapat memberikan saham nya kepada karyawan sebagai bentuk apresiasi loyalitas karyawan dalam berkontribusi kepada perusahaan.
#### Satiscfaction :
  - Perusahaan perlu mempertimbangkan kepuasan karyawan antara kerjaan dengan kehidupan pribadi, hal ini dapat dilakukan dengan perusahaan dapat menyewa psikolog dari konsultan agar karyawan yang burn out bekerja dapat berdiskusi dengan psikolog yang telah disediakan atau perusahaan dapat memberikan bonus tambahan kepada karyawan dengan pergi berlibur dengan rekan kerja di kantor pada saat weekend. 
#### Salary Related :
  - Perusahaan dapat mempertimbangkan untuk kenaikan gaji karyawan di atas 10% dan berikan bonus/ insentif kepada karyawan yang masih bekerja di kantor.
#### Time Related :
  - Perusahaan dapat meningkatkan pelatihan kepada karyawan minimal 1 tahun 1x terutama untuk karyawan yang baru bekerja diperusahaan ini, untuk karyawan yang memiliki perfoma bagus perusahaan dapat mempertimbangkan untuk menaikan jabatan baru minimal 1 tahun bekerja diperusahaan atau 1 tahun mereka bekerja dari posisi sekarang. 
