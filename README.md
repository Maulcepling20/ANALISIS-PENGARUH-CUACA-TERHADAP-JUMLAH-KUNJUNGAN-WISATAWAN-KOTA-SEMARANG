# ANALISIS-PENGARUH-CUACA-TERHADAP-JUMLAH-KUNJUNGAN-WISATAWAN-KOTA-SEMARANG
Analisis ini bertujuan untuk mengetahui pengaruh cuaca terhadap jumlah kunjungan wisatawan di Kota Semarang. Hasilnya bermanfaat sebagai acuan dan evaluasi bagi pengelola pariwisata serta pelaku usaha di bidang wisata. Repositori ini berisi hasil analisis data cuaca di Kota Semarang yang meliputi variabel "Suhu Rata-Rata Kota Semarang", "Kelembapan Udara", "Jumlah Curah Hujan", "Lama Penyinaran Matahari", "Kecepatan Angin Rata-Rata" yang didapatkan dari situs resmi BMKG [Jawa Tengah](https://dataonline.bmkg.go.id/home) dengan satelit yang digunakan yaitu satelit klimatologi Jawa Tengan, dan terdapat variabel "Jumlah Kunjungan Wisatawan Kota Semarang" yang diambil dari situs resmi BPS Kota Semarang. Analisis dilakukan menggunakan Google Colab dengan bahasa Python, serta beberapa package pendukung untuk pengolahan dan visualisasi data.

## Tahapan Analisis
1. **Imputasi Data**  
   - Memanggil dataset dengan package pandas.  

2. **Visualisasi Dataset**  
   - Menampilkan dataset dalam bentuk **tabel**.  
   - Membuat **grafik garis** untuk melihat tren pada variabel cuaca dan jumlah kunjungan wisatawan.  

3. **Pengecekan Nilai Hilang**  
   - Mengecek jumlah dan posisi nilai `NaN` dalam dataset.  

4. **Pengecekan Distribusi Statistik**  
   - Menghitung **mean, median, modus, varian, dan standar deviasi** untuk setiap variabel.  
   - Menyajikan hasil dalam bentuk tabel deskriptif.  

5. **Normalisasi Data (Min-Max Normalization)**  
   - Melakukan skala ulang data agar berada pada rentang [0,1] untuk mempermudah analisis.  

6. **Uji Regresi Linear Berganda**  
   - Menggunakan metode **OLS (Ordinary Least Squares)** dari `statsmodels.api` untuk mengukur pengaruh variabel cuaca terhadap jumlah kunjungan wisatawan.  
   - Menampilkan hasil analisis berupa koefisien, nilai p-value, R², dan uji F.  

7. **Pengambilan Kesimpulan**  
   - Menyimpulkan faktor cuaca yang paling berpengaruh signifikan terhadap jumlah kunjungan wisatawan.  
   - Memberikan interpretasi dari hasil regresi linear berganda.  

## Tools & Packages yang Digunakan
- [Pandas](https://pandas.pydata.org/) → manipulasi data  
- [NumPy](https://numpy.org/) → perhitungan numerik  
- [Statsmodels](https://www.statsmodels.org/stable/index.html) → regresi linear berganda (OLS)  
- [Matplotlib](https://matplotlib.org/stable/) → visualisasi grafik  
- [Seaborn](https://seaborn.pydata.org/) → visualisasi data dengan tampilan statistik lebih informatif  
- [IPython.display](https://ipython.readthedocs.io/en/stable/api/generated/IPython.display.html) → menampilkan output tabel/visualisasi di Google Colab  

## Hasil Analisis
Untuk penelitian selanjutnya, peneliti menyarankan untuk melakukan research kembali terkait variabel-variabel lainnya yang memiliki pengaruh tinggi dan signifikan terhadap jumlah kunjungan wisatawan di Kota Semarang, dengan tujuan untuk meningkatkan hasil akurasi pada prediksi data jumlah kunjungan serta dapat dijadikan sebagai acuan yang lebih kuat untuk bidang pariwisata, khususnya untuk bidang wiraswasta dan pengelola tempat wisata.

