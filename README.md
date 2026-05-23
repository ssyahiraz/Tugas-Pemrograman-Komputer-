# 📊 Tugas Besar Pemrograman Komputer - Teknik Perminyakan

# Profil dan Analisis Project

## Profil Kelompok

### Judul Project

Analisis Produksi Minyak dan Gas Menggunakan Python

### Mata Kuliah

Pemrograman Komputer

### Anggota Kelompok

1. Amanda Sekar Motinda
(27250056)
3. (Gita Anjani) - (27250084)
4. (Putri Hisanaah Nabilah) -
(27250085)
5. Syahira Alya Putri - (27250087)
6. Jobanva Olivia Kezia Putri -
(27250056)

### Deskripsi Project

Project ini dibuat untuk menganalisis data produksi minyak dan gas menggunakan bahasa pemrograman Python pada Google Colab. Analisis dilakukan dengan proses data preprocessing, perhitungan parameter produksi, visualisasi data, dan interpretasi hasil produksi minyak serta gas.

### Tools dan Library yang Digunakan

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Plotly

---

# Analisis Code

## 1. Analisis Gas Oil Ratio (GOR)

Program menghitung nilai Gas Oil Ratio (GOR) untuk mengetahui perbandingan antara produksi gas dan produksi minyak. Pada kode dilakukan pengecekan apakah nilai GOR termasuk tinggi atau rendah.

### Hasil Analisis

Jika nilai GOR lebih besar dari 2000 scf/bbl maka produksi gas dianggap tinggi. Kondisi ini menunjukkan bahwa reservoir menghasilkan gas dalam jumlah besar dibandingkan minyak. Sebaliknya, jika nilai GOR rendah maka produksi minyak masih lebih dominan.

---

## 2. Analisis Penurunan Produksi Minyak

Kode menampilkan data laju produksi minyak dari waktu ke waktu.

### Hasil Analisis

Data menunjukkan adanya penurunan produksi minyak dari 1500 bbl/day menjadi 950 bbl/day. Penurunan ini dapat terjadi karena tekanan reservoir berkurang, umur sumur yang semakin tua, atau berkurangnya kemampuan reservoir dalam mengalirkan fluida ke permukaan.

---

## 3. Analisis Recovery Factor (RF)

Program menghitung Recovery Factor menggunakan rumus:

RF = NP / IOIP

Keterangan:

* NP = cumulative production
* IOIP = initial oil in place

### Hasil Analisis

Recovery Factor digunakan untuk mengetahui seberapa besar minyak yang berhasil diproduksikan dari total cadangan awal. Semakin tinggi nilai RF maka semakin baik tingkat pengurasan reservoir.

---

## 4. Analisis Dataset Produksi Minyak dan Gas

Dataset dibaca menggunakan library Pandas kemudian dilakukan pengecekan isi data dengan fungsi:

* head()
* tail()
* describe()
* info()

### Hasil Analisis

Analisis awal menunjukkan struktur dataset, jumlah data, tipe data, serta informasi statistik seperti rata-rata, nilai maksimum, dan minimum produksi.

---

## 5. Analisis Data Preprocessing

Pada tahap preprocessing dilakukan beberapa proses, yaitu:

1. Mengisi missing value dengan angka 0 menggunakan:

python
fillna(0)


2. Mengubah format tahun menjadi datetime.

3. Mengganti nama kolom agar lebih mudah digunakan dalam analisis.

4. Membuat fitur baru bernama Water Cut.

### Hasil Analisis

Tahap preprocessing membantu membersihkan data sehingga lebih siap digunakan untuk analisis lanjutan dan visualisasi.

---

## 6. Analisis Water Cut

Water Cut dihitung menggunakan rumus:

Water Cut = Water Produced / (Oil Produced + Water Produced)

### Hasil Analisis

Water Cut menunjukkan persentase kandungan air dalam fluida produksi. Jika nilai Water Cut tinggi maka produksi air lebih dominan dibanding minyak. Hal ini biasanya terjadi pada sumur yang sudah tua atau reservoir yang mulai mengalami penurunan kualitas produksi.

---

## 7. Analisis Statistik Produksi

Program menghitung:

* Rata-rata produksi gas
* Produksi gas maksimum
* Standar deviasi produksi minyak
* Produksi kumulatif minyak

### Hasil Analisis

1. Rata-rata produksi gas digunakan untuk mengetahui performa umum produksi gas.
2. Produksi maksimum menunjukkan titik produksi tertinggi pada data.
3. Standar deviasi menunjukkan tingkat variasi produksi minyak.
4. Produksi kumulatif menunjukkan total produksi minyak dari waktu ke waktu.

---

## 8. Analisis Visualisasi Data

Program membuat beberapa visualisasi menggunakan Plotly, yaitu:

### a. Grafik Time Series

Menampilkan perkembangan produksi minyak dan gas berdasarkan waktu.

### Analisis

Grafik menunjukkan tren perubahan produksi dari tahun ke tahun sehingga mempermudah identifikasi kenaikan atau penurunan produksi.

### b. Grafik Top Wells

Menampilkan 10 sumur dengan produksi minyak terbesar.

### Analisis

Grafik membantu mengetahui sumur dengan kontribusi produksi tertinggi sehingga dapat dijadikan prioritas dalam pengelolaan lapangan.

### c. Grafik Scatter Produksi Minyak dan Gas

Menampilkan hubungan antara produksi minyak dan gas.

### Analisis

Scatter plot digunakan untuk melihat korelasi antara produksi minyak dan gas. Jika titik-titik cenderung naik bersama maka terdapat hubungan positif antara keduanya.

### d. Analisis Produksi Gabungan

Gas dikonversi ke BOE (Barrel Oil Equivalent) untuk dibandingkan dengan produksi minyak.

### Analisis

Konversi BOE membantu menyamakan satuan energi antara minyak dan gas sehingga total produksi energi dapat dianalisis secara lebih mudah.

---

# Kesimpulan

Berdasarkan hasil analisis, data produksi minyak dan gas mengalami perubahan dari waktu ke waktu. Tahap preprocessing berhasil membersihkan data sehingga dapat digunakan untuk analisis statistik dan visualisasi. Perhitungan GOR, Recovery Factor, Water Cut, serta visualisasi produksi membantu memahami kondisi reservoir dan performa produksi sumur minyak dan gas.

Penggunaan Python dan library seperti Pandas, NumPy, Matplotlib, dan Plotly sangat membantu dalam proses pengolahan data, analisis, dan visualisasi sehingga hasil dapat dipahami dengan lebih jelas dan sistematis
