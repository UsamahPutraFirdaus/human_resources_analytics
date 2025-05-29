# Menyelesaikan Permasalahan Perusahaan Human Resource

## Business Understanding
Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Selama lebih dari dua dekade beroperasi, perusahaan ini telah berkembang pesat dan kini memiliki lebih dari 1000 karyawan yang tersebar di berbagai daerah di seluruh Indonesia. Namun, meskipun telah mencapai skala yang cukup besar, Jaya Jaya Maju masih menghadapi tantangan signifikan dalam hal pengelolaan sumber daya manusia. Hal ini menyebabkan tingginya tingkat _attrition_, yaitu rasio karyawan yang keluar dibandingkan dengan total keseluruhan karyawan, yang kini telah melebihi angka 10%. Kondisi ini menunjukkan adanya kebutuhan mendesak untuk perbaikan dalam strategi manajemen karyawan agar perusahaan dapat mempertahankan dan mengembangkan tenaga kerjanya secara lebih optimal.

### Business Problem
Tingginya tingkat attrition karyawan (lebih dari 10%) yang mengindikasikan adanya masalah dalam pengelolaan sumber daya manusia, sehingga dapat mengganggu stabilitas operasional dan pertumbuhan perusahaan. Dari masalah tersebut berikut adalah permasalahan bisnis yang akan diselesaikan :
1. Mengidentifikasi faktor-faktor utama yang mempengaruhi attrition rate di perusahaan.
2. Membuat business dashboard yang memudahkan manajemen HR memantau dan menganalisis faktor-faktor penyebab attrition secara berkala.
   
### Project Scope
- Data Cleaning
- Exploratory Data Analysis (EDA) untuk mencari tahu faktor penyebab attrition rate yang tinggi melalui visualisasi data
- Membuat Business Dashboard dari faktor penyebab tingginya attrition rate
  
### Preparation
Sumber data : [Jaya Jaya Maju](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee)

Setup Environment:
1. Clone Repository
   ```
   git clone https://github.com/UsamahPutraFirdaus/human_resources_analytics
   ```
2. Create Python Environment:
   ```
   virtualenv venv
   ```
3. Activate Environment:
   ```
   venv\Scripts\activate
   ```
4. Install the Requirement `requirement.txt`
   ```
   pip install -r requirements.txt
   ```

## Business Dashboard
[Jaya Jaya Maju Dashboard](https://lookerstudio.google.com/reporting/331604dd-32cb-4233-996b-fca7c3e5c751) didesain sefektif mungkin untuk memberikan insight kepada para manajer departemen HR terkait attrition rate yang cukup tinggi hingga lebih dari 10%.

  ![img alt](https://github.com/UsamahPutraFirdaus/human_resources_analytics/blob/main/Usamah%20Putra%20Firdaus-Dasboard.png?raw=true)

Berikut adalah interpretasi dari hasil Dashboard yang telah dibuat:
1. Summary
   - Avg Working: Rata-rata lama bekerja adalah 7 tahun.
   - Avg Promotion: Rata-rata promosi yang diterima karyawan adalah 2 kali dalam setahun.
   - Avg Training: Rata-rata pelatihan yang diikuti adalah 3 kali pada tahun lalu.
   - Avg Salary: Rata-rata gaji karyawan adalah $6,625.95.
     
   Secara umum, karyawan sudah bekerja cukup lama dan telah mendapatkan pelatihan serta promosi, namun masih terjadi attrition yang tinggi. Ini menunjukkan bahwa promosi dan pelatihan belum cukup efektif menurunkan attrition.

2. Gender
   - Laki-laki: 58.6% (620)
   - Perempuan: 41.4% (438)
     
   Komposisi karyawan didominasi oleh laki-laki.

3. Education Field
   - Bachelor: 38.8% (410)
   - Master: 26.1% (276)
   - College: 19.7% (208)
   - Below College: 12.4% (131)
   - Doctor: 3.1% (33)

   Mayoritas karyawan berasal dari jenjang pendidikan S1 (Bachelor), diikuti Master dan College.

4. Marital Status
   - Married: 43.9% (464)
   - Single: 33.3% (352)
   - Divorced: 22.9% (242)

   Sebagian besar karyawan sudah menikah sebanyak 43.9% atau 464.

5. Age
   - Kelompok usia terbanyak: 30–40 tahun (437 orang)
   - Usia 18–30 dan 40–50 juga cukup banyak.
   - Sangat sedikit karyawan berusia 60 tahun ke atas.
   
   Karyawan usia produktif (30–40 tahun) mendominasi. Hal ini penting karena segmentasi ini perlu perhatian ekstra agar retensi tetap tinggi.
   
6. Attrition by Work Life Balance
   - Karyawan dengan work-life balance tinggi tetap mengalami attrition (94 orang).
   - Karyawan dengan work-life balance sedang hingga sangat tinggi juga menunjukkan adanya attrition.
   - Work-life balance rendah (_low_) memiliki jumlah attrition yang paling kecil secara jumlah (18 orang), meskipun kecil namun kurang lebih 30% karyawan yang

   Meskipun Work life balance rendah (_low_) memiliki attrition yang paling sedikit, namun kategori rendah (_low_) merupakan paling banyak secara presentase dibandingkan dengan kategori yang lainnya, dimana kategori rendah (_low_) kurang lebih 30% yang melakukan attrition

7. Attrition by Age
   - Usia 18–30 tahun memiliki jumlah attrition cukup besar (70 dari 236 = ~29.7%)
   - Usia 30–40 tahun juga tinggi (66 dari 437 = ~15.1%)
   - Usia 40–50 tahun ke atas cenderung lebih stabil

   Karyawan muda (18–30 tahun) paling rentan keluar, bisa jadi karena mencari peluang lebih baik atau tidak puas dengan kondisi kerja awal.

8. Attrition by Job
   - Jabatan dengan attrition tertinggi:
     - Sales Executive (39 orang)
     - Research Scientist (38 orang)
     - Laboratory Technician (49 orang)
     - Sales Representative (25 orang dari total 58 = sangat tinggi secara persentase)
       
   Beberapa posisi seperti Sales dan Teknis/Laboratorium memiliki tingkat attrition yang tinggi. Ini bisa mengindikasikan tekanan kerja tinggi, kurangnya penghargaan, atau kurang prospek jenjang karier.

## Conclusion
Berikut adalah point-point penting dari hasil interpretasi diatas:
1. **Usia Muda Rentan Mengalami Attrition** : Kelompok usia 18–30 tahun memiliki tingkat attrition tertinggi secara persentase (~29.7%). Artinya, karyawan muda lebih cenderung keluar, kemungkinan karena mencari jenjang karier yang lebih cepat atau kurang puas dengan kondisi awal kerja.
   
2. **Work-Life Balance Sangat Mempengaruhi Attrition** : Meskipun jumlah karyawan dengan work-life balance rendah tidak banyak, sekitar 32% dari mereka keluar, tertinggi dibandingkan kategori lainnya. Ini menandakan bahwa buruknya work-life balance sangat berisiko meningkatkan attrition.
   
3. **Jabatan Tertentu Memiliki Risiko Tinggi Attrition** : posisi seperti Laboratory Technician 49 keluar dari 188 → ~26.1%, Sales Representative: 25 keluar dari 58 → ~43.1% (sangat tinggi), Sales Executive dan Research Scientist juga cukup tinggi. Posisi tersebut kemungkinan memiliki beban kerja tinggi, tekanan target, atau kurang peluang berkembang.
   
## Recommended Action Items
Berikut adalah Recommended action untuk perusahaan sebagai bahan pertimbangan:
1. Fokus pada Perbaikan Work-Life Balance

   Karyawan dengan work-life balance rendah menunjukkan persentase attrition tertinggi. Perusahaan perlu menerapkan kebijakan yang mendukung keseimbangan kerja dan kehidupan, seperti jam kerja fleksibel, pengurangan beban kerja berlebih, serta dukungan kesehatan mental.

2. Pertahankan Karyawan Muda dengan Program Pengembangan

   Attrition paling banyak terjadi pada usia 18–30 tahun. Perusahaan disarankan untuk membuat program mentoring, pelatihan karier yang menarik, serta memperjelas jalur promosi agar karyawan muda merasa dihargai dan memiliki prospek di perusahaan.

3. Tinjau Ulang Jabatan dengan Tingkat Keluar Tinggi

   Posisi seperti Sales Representative dan Laboratory Technician memiliki risiko keluar tinggi. Perusahaan perlu mengevaluasi ulang beban kerja, sistem insentif, dan kepuasan kerja di jabatan tersebut untuk menekan angka keluar.
