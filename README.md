# 📊 Tugas Besar Pemrograman Komputer - Teknik Perminyakan

## 🧑‍💻 Profil Anggota
* **Nama:** Syahira Alya Putri
* **Program Studi:** Teknik Perminyakan
* **Kampus:** Institut Teknologi Sains Bandung (ITSB)

---

## 🛠️ Deskripsi Code & Analisis Output

### 1. Logika IF/ELSE (Skrining Sumur)
* **Kasus:** Program mengevaluasi nilai GOR saat ini (1200 scf/bbl) terhadap batas kritis (2000 scf/bbl).
* **Output:** `High oil production (Dominan produksi minyak)`
* **Analisis:** Nilai GOR aman di bawah batas kritis, mengindikasikan sumur masih memproduksikan minyak secara dominan tanpa gangguan kebocoran tudung gas (*gas cap*).

### 2. Iterasi FOR LOOP (Monitoring Tren)
* **Kasus:** Membaca data laju produksi minyak bulanan secara berurutan: 1500, 1350, 1100, dan 950 bbl/day.
* **Analisis:** Terdeteksi adanya tren penurunan produksi (*Decline Trend*). Data historis ini penting untuk menghitung laju penurunan sumur guna merencanakan jadwal stimulasi.

### 3. Modul FUNCTION (Kalkulator Reservoir)
* **Kasus:** Rumus otomatis untuk menghitung cepat parameter lapangan.
* **Output Perhitungan GOR:** `1500.0 scf/bbl` (Tiap 1 barel minyak membawa 1500 kaki kubik gas).
* **Output Perhitungan Recovery Factor (RF):** `25.0%`
* **Analisis:** Lapangan baru menguras 25% minyak dari total keseluruhan cadangan di dalam tanah (IOIP). Sisa cadangan masih besar (75%), direkomendasikan merencanakan metode kuras lanjut (*Secondary Recovery* seperti *Waterflood*).
