# Data-Analysis-Capstone-2
---
Analysis yang dibuat berdasarkan data dummy yang diasumsikan sebagai CloudAxis Solution Inc. yang merupakan perusahaan dengan model bisnis SaaS, Analysis ini bertujuan untuk menjawab tantangan dari beberapa problem statement yang sudah dibuat didalamnya, analysis sudah dilengkapi dengan data understanding, visual hingga insights dan rekomendasi.
---
# Harap Download Terlebih Dahulu Semua File Yang Tersedia
---

# BACKGROUND
CloudAxis Solutions Inc. adalah perusahaan SaaS (Software as a Service) multinasional yang berkantor pusat di New York (AS). Didirikan pada tahun 2011, CloudAxis fokus menyediakan berbagai platform software terpadu untuk pengelolaan data, pemasaran digital, solusi keuangan bagi perusahaan lintas industri dan masih banyak lagi.

SaaS (Software as a Service) adalah model penyediaan perangkat lunak berbasis cloud di mana aplikasi dihosting oleh penyedia layanan dan diakses oleh pengguna melalui internet. Pengguna tidak perlu menginstal, mengelola, atau memperbarui perangkat lunak secara mandiri karena semuanya dikelola oleh penyedia SaaS.

NOTE: Pada kasus kali ini data yang akan dianalisis adalah data histori penjualan yang dimiliki oleh CloudAxis Solutions Inc. dimana berikut adalah hal yang akan dianalisis:

1. Profit.
2. Sales.
3. Discount.
4. Order Date.
5. Customer.
6. Subregion.
7. Region.
8. Quantity.

data mentah ini akan dicek terlebih dahulu berkaitan dengan distribusi data, data missing, data outlier, penambahan dan/atau pengurangan kolom, sehingga menjadi data yang bersih dan siap untuk diolah agar hasil dari analisis bisa sesuai dengan yang diinginkan.

Problem Statement : 
1. Bagaimana perusahaan dapat meningkatkan profit dan sales?
2. Bagaimana penerapan diskon yang sudah berjalan?
3. Bagaimana cara mengoptimalkan customer yang ada?
4. Apakah ada ruang untuk melakukan ekspansi?

---

# Goal

Tujuan utama sebagai Data Analyst adalah untuk memberikan insights kepada perusahaan terhadap masalah yang terjadi dan agar dapat mengoptimalisasi kinerja serta meningkatkan profit melalui insights dan rekomendasi langkah yang dihasilkan dari analisis data yang dilakukan.

---

# Stake Holder

Stake Holder untuk hasil analisi data ini ialah Manajemen CloudAxis, yang diantaranya:

1. Business Development
Bertanggung jawab atas strategi penetapan harga, kebijakan diskon, dan peningkatan profit.

Membutuhkan analisis untuk mengevaluasi dampak diskon terhadap profit dan menyesuaikan harga produk.

2. Tim Penjualan (Sales Team)
Regional Sales Manager (EMEA, AMER, APAC): Memantau performa masing-masing wilayah.

Account Executive: Memahami perilaku dan kebutuhan customer mereka.

3. Tim Produk
Product Manager: Melihat produk mana yang paling laris, margin profit, dan feedback pasar.

4. Quality Assurance (QA):
Dengan adanya temuan profit yang negatif tim ini perlu mengetahui dan memastikan barang layak, memenuhi standard dan sesuai dengan demand market untuk memastikan juga bahwa profit negatif terjadi bukan serta merta kesalahan produksi.

5. Customer Support & Services
Dengan kemungkinan berdiskusi dengan customer support and service dapat memberi wawasan tentang POV dari customer dan jika ada perubahan tim bisa menginfokan dengan baik kepada customer untuk menjaga informasi tersampaikan dengan baik dan menjaga hubungan baik dengan customer.

---

# Data Yang Digunakan
Data yang digunakan merupaka data dummy yang terlampir:

- SaaS-Sales.csv
- Saas-Sales-Cleaned.csv

File Analysis:

- JCDS-0808-002-RegiDwiDarmawan _Caps2.ipynb (Jupyter Notebook)
- Visualisasi : JCDS-0808-002-RegiDwiDarmawan  - Caps2.twbx
- SaaS-Sales.csv (Raw Data)
- Saas-Sales-Cleaned.csv (Cleaned Data)
- clv_analysis_result.csv (Additional)

---

# Tools Yang Digunakan
1. Microsoft Visual Studio Code, Jupyter Notebook
2. Programming Language: Python (Pandas, Numpy, SciPy)
3. Visualisasi: Seaborn, Matplotlib
4. Dashboard interaktif: Tableau
5. Presentation: Canva

---

# Langkah Untuk Dapat Menjalankan Kode di Notebook
1. Install Python
2. Install VSCode
3. Open VSCode
4. Pilih open file
5. Open file .ipynb yang sudah di download sebelumnya
6. Install library yang diperlukan
7. Ubah path file menjadi path sesuai lokasi penyimpanan file masing-masing.
8. Run setiap cell yang ada.
9. Selamat Mencoba!

---
# Kesimpulan
# Insights dan Rekomendasi

1. Produk dan Profitabilitas
Insights:

Produk dengan kontribusi profit tertinggi: Alchemy, Site Analytic, Data Smasher, Support, Finance Hub.
Beberapa produk seperti Marketing Suite dan ContactWatcher memiliki penjualan tinggi tetapi profit negatif.
Penetapan harga tidak konsisten, menyebabkan kerugian pada 125 produk yang terjual tanpa profit.
Diskon besar (>50%) diberikan secara tidak terarah, berdampak negatif pada profit.
Rekomendasi:

Fokuskan penjualan pada produk dengan rasio profit tinggi (Alchemy, Support, dll.).
Evaluasi atau hentikan penjualan produk dengan profit negatif.
Tetapkan harga dasar yang konsisten untuk semua produk.
Batasi diskon besar hanya untuk produk yang sepi peminat atau dalam periode tertentu.
2. Strategi Harga dan Diskon
Insights:

Diskon besar (>50%) diberikan secara masif dan tidak terarah, bahkan untuk produk yang tidak terlalu diminati.
Diskon diberikan secara acak tanpa strategi jelas, mengurangi profit.
Beberapa wilayah (APJ, LATAM) memiliki penjualan rendah meski diberi diskon besar.
Pasar EMEA berkontribusi 45.4% penjualan, sementara APJ hanya 18.1%.
Harga jual terlalu bervariatif karena tidak adanya harga dasar menyebabkan kerugian yang besar.
Rekomendasi:

Buat kalender diskon terencana untuk menghindari pemberian promo acak.
Berikan diskon pengenalan di pasar yang tertinggal (APJ, IND, LATAM).
Pertahankan diskon rendah di pasar besar (EMEA, NAMER) untuk menjaga margin.
Gunakan bundling atau cross-selling untuk produk margin tinggi.
Tetapkan harga dasar yang konsisten antar produk untuk meminimalisir kerugian dan arah penjualan yang jelas.
3. Segmentasi Pelanggan
Insights:

Sektor SMB menyumbang 51.6% penjualan, sementara Enterprise paling rendah.
Beberapa pelanggan besar (Allstate) memberikan kerugian meskipun sales tinggi.
Anthem dan Valero Energy memiliki profitabilitas tinggi, sementara Gazprom dan Allstate merugi.
Rekomendasi:

Ekspansi pasar SMB ke wilayah baru.
Lakukan riset untuk meningkatkan penetrasi di segmen Enterprise.
Evaluasi biaya layanan untuk pelanggan dengan profitabilitas negatif (Allstate).
Prioritaskan pelanggan dengan CLV dan profitabilitas tinggi (Anthem, Valero Energy).
4. Tren Musiman dan Wilayah
Insights:

Penjualan lemah di Q1-Q2, tetapi kuat di Q3-Q4 (peak season).
Subregion APAC unggul (500k sales), sementara LATAM, JAPN, ANZ, dan IND tertinggal.
Region APJ jauh tertinggal dibelakang AMER dan EMEA.
Rekomendasi:

Lakukan seasonal promo di Q1-Q2 untuk mendongkrak penjualan.
Tingkatkan penetrasi pasar di wilayah dengan penjualan rendah (IND, LATAM) dengan strategi harga kompetitif.
Identifikasi hambatan di subregion yang kurang berkembang (logistik, persaingan, brand awareness).
Terapkan seasonal promo untuk mendorong penjualan di Q1 & Q2 (low season).
Ekspansi ke wilayah APJ sangat terbuka dan memungkinkan untuk mengulang kesuksesan sepeti di wilayah EMEA.
Penetrasi di wilayah AMER diperlukan dengan riset dan promo agar dapat menyusul angka EMEA.
Kesimpulan Utama:
Tingkatkan Profitabilitas: Fokus pada produk dan pelanggan yang menguntungkan, evaluasi harga dan diskon.
Ekspansi Pasar: Kembangkan segmen SMB dan Enterprise, serta wilayah APJ dan LATAM.
Optimalkan Strategi Promo: Gunakan diskon terarah, bundling, dan seasonal promo untuk meningkatkan penjualan tanpa mengorbankan margin.
Perbaiki Regulasi Harga: Tetapkan harga dasar dan Minimum Order Quantity (MOQ) dibeberapa transaksi jika menggunakan promo khusus untuk meminimalkan kerugian.
Dengan implementasi rekomendasi ini, perusahaan dapat meningkatkan profitabilitas, memperluas pasar, dan mengoptimalkan strategi penjualan.

---
# Presentation Link

https://www.canva.com/design/DAGwbk-5zcc/kSA9gy992wY9yTl-zEAMFw/edit

---

# Data Visualisasi Bisa Juga Diakses Di:
https://public.tableau.com/app/profile/regi.dwi.darmawan/viz/JCDS-0808-002-RegiDwiDarmawan-Caps2/HomePage?publish=yes

---
# Author

Regi Dwi Darmawan
kritik dan saran dapat sangat membantu
kirimkan melalui regi.dwi21.rd@gmail.com
