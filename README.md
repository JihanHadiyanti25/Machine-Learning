# 🎓 Student Performance Analysis & Machine Learning

Proyek ini bertujuan untuk menganalisis faktor-faktor yang memengaruhi performa akademik siswa serta membangun model Machine Learning untuk memprediksi nilai dan kelulusan siswa berdasarkan dataset **Student Performance**.

---

## 📁 Struktur Repository

- `Student_Performance.csv` : Dataset utama yang berisi 25.000 data performa siswa.
- `student-performance.ipynb` : Notebook Jupyter tempat proses Exploratory Data Analysis (EDA), Data Preprocessing, dan Modeling dilakukan.
- `README.md` : Dokumentasi utama proyek ini.

---

## 📊 Penjelasan Dataset

Dataset ini mencakup 25.000 data sampel siswa dengan **16 kolom (fitur)** sebagai berikut:

| Nama Kolom | Deskripsi | Tipe Data |
| :--- | :--- | :--- |
| `student_id` | ID unik untuk setiap siswa | Numeric (`int64`) |
| `age` | Usia siswa | Numeric (`int64`) |
| `gender` | Jenis kelamin siswa (`male` / `female`) | Categorical (`object`) |
| `school_type` | Jenis sekolah (`public` / `private`) | Categorical (`object`) |
| `parent_education` | Tingkat pendidikan orang tua | Categorical (`object`) |
| `study_hours` | Jumlah jam belajar per minggu | Numeric (`float64`) |
| `attendance_percentage` | Persentase kehadiran siswa (%) | Numeric (`float64`) |
| `internet_access` | Akses internet di rumah (`yes` / `no`) | Categorical (`object`) |
| `travel_time` | Waktu tempuh ke sekolah | Categorical (`object`) |
| `extra_activities` | Keikutsertaan dalam ekstrakurikuler (`yes` / `no`) | Categorical (`object`) |
| `study_method` | Metode belajar yang digunakan | Categorical (`object`) |
| `math_score` | Nilai mata pelajaran Matematika | Numeric (`float64`) |
| `science_score` | Nilai mata pelajaran IPA/Sains | Numeric (`float64`) |
| `english_score` | Nilai mata pelajaran Bahasa Inggris | Numeric (`float64`) |
| `overall_score` | Rata-rata nilai keseluruhan siswa | Numeric (`float64`) |
| `final_grade` | Nilai/Grade akhir siswa | Categorical (`object`) |

---

## ⚙️ Langkah-Langkah Analisis & Preprocessing

1. **Pembersihan Data (Data Cleaning):**
   - Menghapus data duplikat (`df.drop_duplicates()`).
   - Penanganan *missing values* (jika ada).
2. **Feature Encoding & Preprocessing:**
   - Mengubah variabel biner seperti `internet_access` dan `extra_activities` dari bentuk teks (`yes`/`no`) menjadi numerik (`1`/`0`).
   - Melakukan *encoding* untuk variabel kategorikal lainnya (`gender`, `school_type`, `study_method`, dll.).
3. **Exploratory Data Analysis (EDA):**
   - Menganalisis korelasi antara jam belajar (`study_hours`) dan persentase kehadiran (`attendance_percentage`) terhadap `overall_score`.
4. **Machine Learning Modeling:**
   - Pemisahan data latih dan uji (*Train-Test Split*).
   - Pelatihan model prediktif.

---

## 🚀 Cara Menjalankan Proyek

1. **Clone Repository ini:**
   ```bash
   git clone [https://github.com/JihanHadiyanti25/Machine-Learning.git](https://github.com/JihanHadiyanti25/Machine-Learning.git)
